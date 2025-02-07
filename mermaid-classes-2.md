

```mermaid
classDiagram
    class evlist {
      perf_evlist: core
    }

    class evsel {
      perf_evsel : core
      evlist : evlist
    }

    class perf_evlist {
      list_head : entries
      int : nr_entries
    }

    class perf_evsel {
      list_head : node
      perf_event_attr : attr
    }

    class perf_event_attr {
      __u32 : type
      __u32 : size
      __64 : config
    }
    note for perf_event_attr "'.config' encodes the raw PMU event"

    class perf_event_attr

    class perf_session {
      perf_header : header
      evlist : evlist
    }

    class perf_header {
      perf_header_version : version
      u64 : data_offset
      u64 : data_size
      u64 : feat_offset
      perf_env : env
    }

    class perf_env {
      char * : hostname
      char * : os_version
      char * : version
      char * : arch
      int : nr_cpus_online
      int : nr_cpus_avail      
    }

    class list_head {
      list_head : next
      list_head : prev
    }
    note for list_head "Generic list object added to other objects"

    %% -------------------------------------------
    %% Define relationships

    evlist --> perf_evlist
    evsel --> perf_evsel
    evsel --> evlist
    perf_evsel --> perf_event_attr
    perf_evlist --> list_head
    perf_session --> perf_header
    perf_header --> perf_env

```
