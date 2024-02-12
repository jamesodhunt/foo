<details>
<summary>Click the icon to show the list of commits included in this release</summary>
fcd005774 tools: avoid rootfs-image build "ln -s" error
05c4c8055 runtime-rs: Configure argument replacement for QEMU in Makefile
27cb30d8c runtime-rs: Adjust configuration template for runtime-rs
462afcf82 runtime-rs: Copy configuration for QEMU from runtime
f139c7dc6 tests: k8s: k8s-copy-file auto-generated policy
1179306af tests: k8s: additional policy testing utilities
9a780aa98 genpolicy: improve logging from ExecProcessRequest
dab567bdf genpolicy: add easy way to allow CloseStdinRequest
8401adb11 genpolicy: update default values
ff1ace1c7 docs: Remove jenkins reference in kernel documentation
97fbf360c gha: Cleanup nydus snapshotter by the daemonset
43b04fd0c gha: Deploy nydus snapshotter by the daemonset
0b508f301 tests:k8s: make add_kernel_initrd_anotations function generic
a43edd0c3 rootfs: Install pause image into rootfs
42ef6bdca osbuilder:rootfs: support to unpack pause image to rootfs
53183cba3 workflow: Enable to build pause image in ci
70a84eca9 packaging: allow to pull and unpack pause image
3e383674f runtime: fix creation of SEV confidential container on SNP enabled host.
6346e04cf runtime-rs: fix handling of TTRCP_ADDRESS
f0256fded runtime-rs: remove validation of shim v2 -address value
34c47e08b runtime-rs: fix assert error in test in `make check`
6b5e57f7c tests: k8s: address PR review feedback
dd16bc393 tests: k8s: k8s-attach-handlers generated policy
0de407f8b tests: k8s: enable AUTO_GENERATE_POLICY
05b2e4f60 tests: k8s: install genpolicy
8aa8b7057 tests: k8s: add policy test utilities
24a17a2e1 tests: k8s: output the names of test files
bf533de31 tests: k8s: add DEBUG support for test scripts
1b4ef672e tests: k8s: reduce namespace name duplication
8a5ba5fb3 tests: k8s: allow run_kubernetes_tests.sh exec
473efc214 genpolicy: mount source for non-confidential guest
d0b8e6d8f nydus: Bump nydus snapshotter version to v0.13.7
b3c74411f runtime-rs: Add tests for persist api for clh
0b78296dc runtime-rs: Store additional field for hypervisor state
a5f0b92bc runtime-rs: Add guest protection to hypervisor state
ed6816e29 kata-manager: Add support for nerdctl installation
31813cf8d metrics: Update packages for TensorFlow ResNet Int8 Dockerfile
cf049fc71 k8s: Skip k8s tests that are not working
eb5b7d3bf tests: k8s: Enable tests for cloud hypervisor runtime-rs
40b2b2a43 gha: Run static-checks on self-hosted runners conditionally
a214bd8d1 gha: Enable nydus snapshotter in CoCo ci tests
ce82b5e3f rootfs: Add libtdx-attest into the confidential rootfs
106e1af49 cri-containerd: fix loop in TestContainerMemoryUpdate()
e59d00556 gha: add GOPATH env var to the ppc64le k8s workflow
6068faf40 runtime: failed to run in the case of ColdPlugVFIO
27e797404 rootfs: confidential: Install coco-guest-components
f80dbcee0 rootfs: Add logging about the coco guest components
68b8186ec osbuilder: Expose COCOGUEST_COMPONENTS_TARBALL
64d09874c packaging: coco-guest-components: Pass DESTDIR to the build script
d4a9856a8 gha: Remove SEV / SNP / TDX images / initrds
e4258d869 runtime: Use confidential image / initrd instead of TEE specific ones
f354beb25 static-checks: Install clang in the ci environments
c6830ceb8 runtime: display accurate error msg to avoid misleading users.
7bf1ebe16 kata-monitor: fix agentUrl from containerd shim
a04b215bc gha: delete azure RG only if it exists
a9f8888c1 packaging: Add confidential image / initrd
e9de0ef6b packaging: rootfs: Depend on kernel-confidential tarball
b58cfc765 packaging: Ensure rootfs is rebuilt in case kernel changes
4394dacb8 packaging: Build the confidential kernel with MEASURED_ROOTFS support
c7680839f packaging: Fix modules tarball for nvidia-gpu-confidential
dc027e39d gha: Remove TEE specific kernel build targets
3755c6916 runtime: makefile: remove SNP specific kernel references
57b132f94 runtime: makefile: remove SEV specific kernel references
2562d2324 runtime: makefile: remove TDX specific kernel references
f4e3c936d runtime: snp: config: Use the confidential kernel
8731366d7 runtime: sev: config: Use the confidential kernel
6cbdba726 runtime: tdx: config: Use the confidential kernel
a618461d3 runtime: Add confidential kernel to the makefile
6771ca463 gha: k8s: Add cloud-hypervisor (runtime-rs) support
2ff3f0afc packaging: Remove trailing whitespace from extra_tarballs arg
228bc48c7 packaging: Fix kernel confidential name
31b21093b packaging: Pass the kernel flavour to get_kernel_modules_dir
51b1df233 packaging: Fix typo to get the extra_tarballs path
4876eadd2 tools: Add reference to the kata webhook's README
b0b7748f3 ci/openshift-ci: Correct the lib location
4c5847853 ci/openshift-ci: Move openshift-ci from the tests repo
0b221b561 packaging: Fix pushing artefacts to the registry
9317e23df mount: Reduce the mount points with namespace isolation
bb6f5073a runtime-rs: Allow compilation for s390x
8fcee6e6e runtime-rs: Use Persist::restore() of QEMU for VirtSandbox
56aef3741 runtime-rs: Exclude hypervisors plugins except QEMU for s390x
5d2906c36 packaging: Bump the kata config kernel version
d2ea11dbf packaging: Use the cached kernel modules
e5bca9027 packaging: Cache the kernel modules
f481f5865 packaging: Create the tarball for the kernel modules
a58caca72 packaging: Take extra tarballs in install_cached_tarball_component()
33ac5468f packaging: Add function to get the kernel modules directory
f8585db8d gha: add kubernetes tests workflow for ppc64le
0ace31f04 ci: aks: switch from eastus2 to eastus region
09ea0eed9 genpolicy: ignore empty YAML as input
f0339a79a genpolicy: support non-default namespace name
222de4f68 agent: Fix a race condition in passfd_io.rs
6e4d4c329 agent,runtime-rs: Add license header to passfd_io.rs
1206de2c2 agent: Use pipes as stdout/stderr of container process
f6710610d agent,runtime-rs,runk: fix fmt and clippy warnings
89be42a17 runtime-rs: open stdout and stderr fifos NONBLOCK
3eb4bed95 agent: use biased select to avoid data loss
7874ef5fd agent: set stdout/err vsock stream as blocking before passing to child
cfb262d02 container: keep the io connection when pass fd to hybrid vsock
4a762fcfd dbs: hybrid stream support keep the connection when local closed
553674336 agent,runtime-rs: fix container io detach and attach
657b17a86 runtime-rs: open stdin fifo with RDWR|NONBLOCK when pass vsock streams
f1b33fd2e agent: clean up term master fd when container exits
b8632b403 dragonball: vsock: properly handle EPOLLHUP/EPOLLERR events
442df71fe agent,runtime-rs: refactor process io using vsock fd passthrough feature
eb6bb6fe0 config: add two options to control vsock passthrough io feature
973b5ad1f runtime-rs: make Container::new async
b0b8523ce runtime: modify ValidCgroupPath unit test
feed5c8ff runtime: merged ValidCgroupPath method
9aa1ed805 runtime: add SingleContainer when obtaining OCI Spec
864389c52 runtime-rs: report error on missing or empty fields in configuration
531a11159 genpolicy: allow separate paths for rules and settings files
78b517ccc tests: Re-arranged nerdctl tests
d12875ee6 genpolicy: ignore volume configMap optional field
abc2fcd88 kata-deploy: fix deprecations on kustomization files
2e1d770fc packaging: Track files correctly  when naming builder image for agent
f3bc6e415 packaging: Use Ubuntu 20.04 for building an agent
d53edbd0a runtime-rs: collect qemu stderr and log it in shim log
684d74012 runtime-rs: switch qemu child process management from std to tokio
b52a39846 runtime-rs: move creation of VM path from start_vm() to prepare_vm()
3fd562877 dragonball: fix noop-method-call warning
60ac3048e genpolicy: fix ConfigMap volume mount paths
34d51b05f gha: cri-o: Bump runners to 22.04
9b7c5c69c runtime-rs: fix unused driverInfo error
8ad5459be genpolicy: optional PodTemplateSpec metadata field
076869aa3 genpolicy: ignore the nodeName field
98dc2d4c5 rootfs: agent: Initialise AGENT_SOURCE_BIN & AGENT_TARBALL
5e57e0235 rootfs: agent: Fix build with AGENT_SOURCE_BIN
fbfc880eb rootfs: Add COCO_GUEST_COMPONENTS_TARBALL env var
644abde35 packaging: coco-guest-components: Allow building the project
ab597a4d5 opa: Improve the download logic
448c0aaec gha: azure: Set the correct subscription to the account
08a082ca4 gha: Cache the agent for non-x86_64 arches
535cf04ed genpolicy: add shareProcessNamespace support
ab462a4b8 tests: Add IBM SE to the basic confidential test
95c569b0a packaging: Add safe.directory to the git config
dd4947982 packaging: Don't build the agent if not needed
21fd7e6df packaging: Fail in case oras can't find an artefact
eb7a33ee7 rootfs: Always strip the agent binary
f23451de0 rootfs: Add xz as a dep
830771884 rootfs: Add AGENT_TARBALL env var
5b0d0687e packaging: agent: Allow building in all arches
1039641ab packaging: agent: Add the arch to the builder container
58874f9c3 packaging: tools: Add the arch to the builder container
19ecdbca3 qemu: enable TPM
98b5a19b3 tools: Use defined variable in build base qemu script
eb7e123de metrics: Update packages needed for ResNet50 FP32 Dockerfile
723c76d94 tools: allow all users to execute genpolicy
66c012d05 tests: k8s: bats --show-output-of-passing-tests
4b8d79c1f gpu: remove GHA target first then remove the obsoleted Makefile targets
1b0d12ab7 versions: Update libseccomp to version v2.5.5
25ecca91c docs: provide a guide for how to use IBM Secure Execution
a4b208a71 runtime: remove SharedVersions field dead code
4fc34323a gpu: Add NVIDIA GPU Confidential kernel target
ea9c659d3 gha: get ready to install genpolicy
069680738 versions: Update firecracker version
ca03d4763 genpolicy: ignore pod DNS settings
25c8d5db5 runtime-rs: use qemu cmdline generation framework to launch VM
f550d9a32 runtime-rs: add basic implementation of qemu command line generation
e8e13044d runtime-rs: add simple impls to some of Qemu's Hypervisor functions
0cfb2d257 runtime-rs: add simple Persist implementation for Qemu
45862aeec runtime-rs: add default rootfs type for qemu
f6fea5f2c agent: fix failing unit tests on ppc64le
610f87889 dragonball: Fix compile error for aarch64
376941cf6 kata-ctl: skip building kata-ctl on ppc64le
4ecd82a5d runk: skip the test_init_container_create_launcher if not root on ppc64le
a4b544792 tools: fix makefile spacing
394777291 runtime: fix failing unit tests on ppc64le
486b8a053 dragonball: skip running static-checks for ppc64le
14934c7b0 github: run static checks on ppc64le
8061a49ca kata-ctl: Clean up a test leftover file explicitely
290ecf4c4 Static-check: Exclude s390x from dragonball and runtime-rs
c0f57c9e0 Lint: Fix `cargo clippy` errors for s390x
a1f288e5d CI: Use sudo if yq_path is not writable by USER
354cbede9 GHA: Enable static check for s390x
ba74a624a runtime-rs: use pathBuf only for x86
a10779bf0 GHA: enable static check on arm64
febabef08 tools: install genpolicy settings files
7da6d0a84 runtime-rs: ch: Implement missing thread/pid APIs
f4106a610 genpolicy: use root path from cbl-mariner Guest VM
4b772d248 tests: Ignore virtiofs contribution to memory usage when it is disabled.
201eec628 tools: genpolicy static checks
205dafd32 genpolicy: temporarily disable allow_storages()
99717371c runtime-rs: bugfix for DirectVolume/rawblock when driver is blk
dff800a8f metrics: Remove iperf3 server protocol
681cb1626 genpolicy: cargo clippy fixes
b7c31e3b9 tests: cbl-mariner: disable k8s-oom.bats
f1fda3d6b dragonball: Remove unused definition
dcaae54cf genpolicy: "cargo fmt -- --check" clean-up
12a41f89b metrics: Use a specific python version to run tensorflow benchmark
b97efc313 CI: enable test container memory update for dragonball
6c85e95c3 CI: bugfix for dragonball when CI running with cri-containerd
cd59d31a1 CI: make CI work for dragonball to test stability and cri-containerd
29e0de4e4 runtime-rs: ch: Implement minimal memory hotplug APIs
1c0df670a runtime-rs: ch: Add minimal implementation of hypervisor metrics method
6bac3323b workflows: Update backport-label to use gh-utils.sh
0d5d1c8c3 ci: Add gh-util.sh script
080541a0f genpolicy: add SPDX license header
7f126be67 genpolicy: Update oci_distribution to 0.10.0 Also support alternative media type and update samples
9eb6fd4c2 docs: add agent policy and genpolicy docs
57f93195e genpolicy: add support for StatefulSet YAML input
35958ec9c genpolicy: add support for ReplicationController
7da17099f genpolicy: add support for ReplicaSet YAML input
d84300f1e genpolicy: add support for List YAML input
a03452637 genpolicy: add support for Job YAML input
2dbd01c80 genpolicy: add support for Deployment YAML input
a40a6003d genpolicy: add support for DaemonSet YAML input
48829120b policy: initial genpolicy commit
61fe20cf9 gha: Fix some of gha metrics failure for StratoVirt
540a2a7fb runtime: Allow no initrd path for IBM Z Secure Execution
6fd49f760 runtime-rs: Forward events to containerd via ttrpc
e69f7c07a versions: Update runc version
c3f6eaa26 build-kernel: Fix typo 'terball' -> 'tarball'
8b2f43a2c build: Add "confidential" kernel
379e2f3da kernel: update some configs based on kernel 6.5 and 6.6
cf4835e3a packaging: qemu: Simplify "--disable-virtiofsd" logic
bfc6fc7a8 build: Get rid of QEMU experimental
d2080fd22 runtime-rs: refactor getting the vfio device guest pci path
d795fcfc2 runtime-rs: bridge the vfio device between runtime-rs and dragonball
90c782f92 tests: list the current k8s pods
24fab19f6 tests: Remove check images function from stressng test
aceba94d9 tests: Add check images as part of install dependencies
7d41c97f6 packaging: Fix indentation of build static stratovirt
7c176a62f agent: use method params instead of const params in functions
0e9d73fe3 agent: Fix an issue reporting OOM events by mistake
7d5336aca agent: hold lock while setting new policy
4ad1971a0 tests: Add hypervisor component to kill kata components function
44b5b88f4 docs: Update docs for new StratoVirt VMM introduction
4bc67dba0 metrics: Improve iperf3 cleanup
4c023e341 dragonball: Fix compilation issue without all net features
f97f16a44 agent-ctl: Bump ttrpc version
bf59c7b3d runtime-rs: Bump ttrpc and containerd-shim-protos versions
cf9a0e21a protocols: Bump ttrpc version
91360e7dd agent: Bump ttrpc version
f1235ddba dbs_virtio_devices: add Cargo.lock
02cd726bf dbs-utils: add Cargo.lock
97bdc1529 dbs-pci: introduce Cargo.lock
71c322c29 runtime-rs: fix ci complains
f9e0a4bd7 upcall: introduce pci device add & del kernel patch
a3f7601f5 dragonball: add pci hotplug / hot-unplug support
0f402a14f dragonball: add InsertHostDevice vmm action
8779fe7dd runtime-rs: create a reference that directs users to kata csi doc
ba5437382 runtime-rs: add examples about Kata pod with directvol by CSI.
c6d2a3214 runtime-rs: add support for directvol csi deploy scripts.
25d8e83e4 runtime-rs: Add dedicated CSI driver for DirectVolume support in Kata
3b317e69e runtime-rs: add README and user guide to deploy directvol CSI Driver
ea69c1700 runtime-rs: initialize pcie topology in Device Manager
b42548b8e runtime-rs: do unregister device in Trait Device/detach
0f0b6d13c runtime-rs: do register/update device in Trait Device/attach
ce7d36369 runtime-rs: Introduce helper macros to simplify PCIe device ops
0d4992b24 runtime-rs: add one more argument in Device attach/detach
b425de610 runtime-rs: implement Trait PCIeDevice for pcie/pci device
87e39cd1f runtime-rs: introduce Trait PCIeDevice to do [un]register device
6ebc4884f runtime-rs: introduce PCIe Topology framework for pcie/pci devices
88839026b runtime-rs: introduce TopologyConfigInfo to initialize pcie topology
6ee7fb540 kata-deploy: Double quote the snapshotter name
8332f3c68 kata-deploy: Fix the snapshotter config placement
907f1ddb9 kata-deploy: Fix shim check for snapshotter configuration
2f797a6eb pci: rename 2 parameters to follow rust naming convention
9c13b2c99 dragonball: introduce vfio support
81ab174c1 dragonball: support vhost-user-blk in device manager
ef8dc3b0c dragonball: support vhost-user-blk
23eb3042c kata-monitor: fix Dockerfile to build image
36a4cbccf runtime-rs: Expand all DeviceType in match arms
f2d08bc00 runtime-rs: Remove unused index from Endpoints
60a42351e runtime-rs: DAN supports vhost-user-net device
693a0cfbf dragonball: Make vhost-user-net ready for VhostUserEndpoint
54df83240 runtime-rs: Support VhostUserEndpoint
374c2f01a runtime-rs: Simplify VhostUserType enum
4c5de7286 dragonball: Wrap config space into `set_config_space`
beadce54c dragonball: Support vhost-user-net devices
1f21d3cb2 dragonball: Introduce address space for MmioV2DeviceState
94c83cea8 runtime-rs: Refactor vfio driver implementation
82d3cfded runtime-rs: Make VhostUserConfig's field pci_path type more specific
5cc2890a1 runtime-rs: refactor and re-implement pci path.
1b5758c1f runtime-rs: Move the PciPath-related code to a dedicated file
275de453d runtime-rs: remove useless get_host_guest_map and its test case
4a95c0d07 kata-deploy: snapshotter typo fixes
8cf3bcefd dragonball: introduce pci msi/msix interrupt
6cc6ca5a7 kata-deploy: Allow setting up snapshotters per runtime handler
206ed6d77 tests: Load vhost modules explicitly while Kata installing
9f394f6e1 tests: Use function from Kata repo
8aa390279 tests: retry connection to pod SSH server
c9e631dc0 kata-deploy: Reapply "kata-deploy: Use tomlq to configure containerd"
41320c586 kata-deploy: Install jq from GitHub
ee5fa08a2 Revert "kata-deploy: Use tomlq to configure containerd"
9e718b4e2 gha: kata-deploy: Add containerd status check
458e91b28 runtime-rs: Update readme to indicate cloud-hypervisor support
1469a5efc tests: k8s: Fix indentation in confidential common script
551a50cd7 tests: additional run-runk logging
039fe7f39 dragonball: Trigger unit tests of dbs_* subcrates by `make test`
3cd0cc138 runtime-rs: Separate init_config() from new() for struct VsockDevice
b785ef96e docs: Change location of static checks script
bfb756199 ci: Use static checks from kata repo for lib functions
58e88d946 agent: correct CPUShares and CPUWeight value
5637f11a8 kata-ctl: Add option to dump config files
510bc36a7 github-actions: Remove ignore paths for required CI checks
9a37e77f2 runtime-rs: check the update memory size
603941710 runtime-rs: add default_maxmemory in config file
8d9fd9c06 runtime-rs: support memory resize
81e55c424 runtime-rs: add resize_memory trait for hypervisor
d428a3f9b runtim-rs: get guest memory details
c92b14da9 tests: k8s: Fix indentation in setup script
8151117f7 metrics: Improve latency network cleanup
23f76653e metrics: Update command to run the tensorflow int8 benchmark
8fd5ef7fb metrics: Update TensorFlow ResNet50 Int8 Dockerfile
dfad0e662 .github: fix the failure without devicemapper for host sharing
983479748 .github: fix error when making checks for CoCo guest pull
af4622fcc docs: Remove warning for cgroupsv2 only operating systems
0db820fa0 gha: add a post cleanup script for cri-containerd ppc64le workflow
aa42f0a03 runtime-rs: Enhancement of DirectVolume when using CSI.
80d631ee8 runtime-rs: Add attribute serde rename to each field of DirectVolume.
82fde4431 dragonball: Set default queue config for vhost-net device
c11b06672 runtime-rs: Use vhost-net device by default
05e278de5 GHA: Put all the preliminary steps into pre-action for s390x
b46cb2227 static-checks: Direct Makefile to use new static checks
63636b869 static-checks: Update copyright dates
b11c77286 static-checks: Change dir for building tools
a9d360728 static-checks: Fix directory for github labels
7ad873cf2 kata-deploy: Simplify shim configuration
e61894993 kata-deploy: Remove useless comment from CRI-O drop-in
dd9f5b07b kata-deploy: Use tomlq to configure containerd
4f01f294b kata-deploy: Install `tomlq` to the base image
39f5cea3b kata-deploy: Fix k0s cri notation comment
b079e1aab dragonball: add pci root bus and root device
2a518f089 runtime-rs: ch: Change state when VM stopped
1195692d3 runtime-rs: ch: Move state handling to top-level APIs
86918e91b dragonball: Disable packed virtqueue for vhost-user devices
1662a3e85 common: Add cloud hypervisor in enabling hypervisor function
f3eeab10a tests: nerdctl: Enable nerdctl tests for cloud hypervisor runtime-rs
b2577000e metrics: Expose iperf3 pods over a k8s networks.
a062ba166 metrics: cleans k8s iperf deployment when the test finishes.
52f7a40e4 dragonball: add --all for fmt ci
ce694b905 tests: Fix indentation of gha-run script
33b300431 tests: Enable but do not run k8s tests for cloud hypervisor
acee3d843 gha: k8s: Add cloud-hypervisor (runtime-rs) support
375c787e0 rootfs: build OPA binary from source for ppc64le and s390x
28c3e0e5f GHA: Fix kata-deploy-runtime-classes-check for kata-qemu-se
5d085a304 CI: static-checks: Try multiple user agents
3174c1877 docs: Remove problematic URL
3779261a9 docs: Fix whitespace
613def032 CI: static-checks: Move curl to a separate function
6d859f97e CI: static-checks: Lint fixes
efa8e6547 CI: static-checks: Check params have a value
563ea020b CI: static-checks: Fold long line
3ad43df94 CI: static-checks: Improve markdown checker test
40f0c8fbb GHA: Use --client=true for k3s kubectl version
bf97051f1 runtime-rs: fix panic when hypervisor mismatches with configuration
69fdd05ce kata-ctl: Moved log-parser-rs into kata-ctl
636eef890 GHA: make secrets inherited for build-kata-static-tarball-s390x
5629b7454 dragonball: support vhost-user-fs in device manager
2a1fc29e8 dragonball: add unit test for vhost-user-fs
d6cfbe943 dragonball: support vhost-user-fs
3fab1690a local-build: make strip support for cross-compilation
f38c7f14c gha: remove build redundancy of kernel and rootfs-initrd
31db56207 local-build: add support for key verification for IBM Secure Execution
52bdc87fe local-build: make kernel parameters configurable
9ceb2c27e local-build: consider cross-compilation env
511dd5fea local-build: add support to build IBM Z SE image
4de8ef3d1 local-build: add build target boot-image-se
a63a6959d local-build: install s390-tools in Dockerfile
6d0dabd81 gha: build secure image for s390x release
bb1d4adaa config: add SE configuration
8de4241d3 kata-deploy: add kata-qemu-se runtimeclass
9ede2bcd9 local-build: differentiate build targets based on architecture
a661ac3a0 runtime-rs: Implement and use try_from for DiskConfig
50a5fa9a6 tests: Enable but do not run the nerdctl tests for cloud hypervisor
e70b2ea95 gha: nerdctl: Enable cloud hypervisor runtime-rs for nerdctl CI
56dddab04 metrics: Update command to run tensorflow resnet fp32 benchmark
62fdebeeb metrics: Update TensorFlow ResNet FP32 dockerfile
0d5a970e5 GHA: remove GITHUB_WORKSPACE when workflow fails due to merge conflict
16380558e deployment: Create a stable overaly for kata-deploy
955dec06d runtime-rs: add network hotplug for clh
61b868692 docs: Update config containerd url link
b816dca3e image-builder: fix incorrect part start position
a14f2fc18 gha: runk: Fix typo in the test name
1a74142a1 gha: basic-ci: Add a timeout for the tests
48bdca4c4 tests/k8s: add k8s-measured-rootfs.bats
1eae657b9 tests/k8s: add set_node() to lib.sh
c6075c862 tests/k8s: add setup common
220a2d9a1 tests/k8s: add assert_logs_contain() to lib.sh
9a9c7a5c6 tests/k8s: add set_metadata_annotation() to lib.sh
a13eecf7f runtime(-rs): add clean-generated-files target
36ea1b8ee tests/k8s: add new_pod_config() to lib.sh
428daf9eb tests/k8s: add utilities functions for the tests
ba4f806c3 initramfs: re-wrote devices checking on init.sh
72ef82368 shim-v2: ensure root hash exist when measured rootfs
1465e5885 kernel: ensure initramfs exist when measured rootfs
4dbba5215 shim-v2: moved measured rootfs logic to its builder
34be78df1 kernel: moved measured rootfs logic to its builder
3f16d2959 kernel: measured rootfs as argument to build-kernel.sh
05ce52d74 devmapper: dragonball: Enable, but do not run, the tests
a8a156b1a stability: dragonball: Enable, but do not run, the tests
16ad721ed cri-containerd: dragonball:  Enable, but do not run, the tests
1cd1558a9 mount: support checking multiple kinds of block device driver
d62789397 runtime-rs: Show config files attempted on config load failure
45c0364d4 runtime-rs: Fix typo in task service
0fabfa336 runtime-rs: bring support for legacy vsock device.
6c08cf35d runtime-rs: Introduce prepare_vm_socket_config to VirtSandbox.
60f88da5e runtime-rs: add Capability of HybridVsockSupport for Hypervisor.
c5178dd25 runtime-rs: Introduce Capability of HybridVsockSupport.
6af059227 runtime-rs: Add vsock device in device manager.
1a6b45d3b runtime-rs: Reintroduce Vsock and add it to the DeviceType enum
e31dbc94a runtime-rs: remove vhost_fd from VsockConfig and make it cloneable.
eb90962b2 runtime-rs: introduce a new function generate_vhost_vsock_cid.
2df8144cf runtime-rs: Launch cloud-hypervisor in given netns
2b0502934 docs: Update cri installation url link
9166d0aab docs: Update iperf3 network documentation
dfc07d1c7 gha: stability: Add cloud-hypervisor (runtime-rs) support
03c3f4275 kernel: Add CONFIG_TDX_GUEST_DRIVER to the tdx.conf
e1caca3e4 kata-ctl: Remove root requirement for "env"
f05ada592 libs: protection: x86_64: drop root requirement for querying
b3da71f21 dragonball: init dbs-pci lib with pci bus & pci conf
fe68f25be runtime-rs: enhancement of vfio volume.
e3fd40312 runtime-rs: enhancement of spdk volume.
f97372902 runtime-rs: Enhancing DirectVolMount Handling for current Infra.
e3becea56 runtime-rs: add support kata/multi-containers sharing one vfio volume.
b952c5c5c runtime-rs: add support kata/multi-containers sharing one spdk volume.
17d2d465d runtime-rs: re-organize the volumes with adding new direct_volumes.
6731466b1 runtime-rs: set a standard NotFound when direct volume path not found.
d23867273 runtime-rs: split the block volume into block and rawblock volume
f9f1d3a07 libs:logging: Fix logger
8fd39d11c tests: Adapt `enable_hypervisor`to the runtime-rs config location change
38183acbc tests: Use `kata-ctl` instead of `kata-runtime` for runtime-rs
a5a73a11c tests: Replace `kata-runtime kata-env` by `kata-runtime env`
30acb5a0c tests: nydus: Adapt the default config file for runtime-rs based drivers
61aa84b15 Revert "tests: k8s: Allow passing rust-runtime env var to kata-deploy"
158ca17ae kata-deploy: Add cloud-hypervisor
d4e00238a kata-deploy: Improve the logic for linking to the rust runtime
fc28deee0 kata-deploy: Use rust runtime config files in runtime-rs directory
80860478b runtime-rs: Remove the golang config paths
b86ab5aa2 runtime-rs: Update list of config paths to check
89ef464b7 build: Install rust config files to runtime-rs directory
05efb2326 tests: update go.mod and go.sum
6d9cb9325 tests: update scripts for static checks migration
66f3944b5 tests: move github-labels to main repo
7f3c12f1d tests: move spell check tool to main repo
8ad433d4a tests: move markdown check tool to main repo
eaa6b1b27 tests: move static checks and dependencies from tests
98aa291c9 runtime-rs: Add Hybrid VSOCK device handling for CH
37633d3cc metrics: Fix iperf parallel bandwidth limit
96deea52f tests: more k8s-exec-rejected debug output
811ec0735 osbuilder: add pkg bash for alpine
47b8c3181 runtime: remote hypervisor updates to ttrpc
613c75ba8 runtime: Update hypervisor generated code
6a922f0e3 gha: fix artefacts build on ppc64le
1284b4e80 tools: Stop building / shipping log-parser-rs
f15e16b69 Revert "runtime: confidential: Do not set the max_vcpu to cpu"
8839ca93b gha: Disable stratovirt for gha metrics
754aec02c gha: add cri-containerd workflow for ppc64le
4a4fc9c64 CODEOWNERS: Expand scope
5318afe27 runtime: support to create VirtualVolume rootfs storages
0b4f7c2ee runtime: redefine and add functions to handle VirtualVolume to storage
bd099fbda runtime: extend SharedFile to support mutiple storage devices
e4f33ac14 runtime: add functions to create devices in KataVirtualVolume
ae2c0c569 github: add workflows for building and publishing kata artifacts on ppc64le
d8a8cc449 tools: install oras from source on ppc64le
08f360312 tools: fix static build of qemu and shimv2 on ppc64le
4aaf54bda runtime: Fix configmap/secrets update propagation with FS sharing disabled
37916e7a5 metrics: Fix result finding
6de01eacf kernel: backport erofs patch to 6.1.52 guest kernel
44899d4cd tests: k8s: Allow passing rust-runtime env var to kata-deploy
a9571398a dragonball: add test utils for vhost-user
a6a399d5b dragonball: add vhost-user connection management logic
fe62e656a runtime-rs: Name the ShareFs Mount Option type more accurately
856315ff8 runtime-rs: bringing virtio-fs device in device-manager
4d65c2e8a runtime-rs: introduce `update_device` in trait Hypervisor
1353b14e6 runtime: Add KataVirtualVolume struct in runtime
1699b84f1 utils: kata-manager: Remove $enable_debug from the install_kata call
38d2edd83 utils: kata-manager: Allow installing kata from a given tarball
ebf9d2725 kata-deploy: Add remote shim
d5cf169ad kata-deploy: Add missing kata-remote runtimeclass
39e8c8426 runtime: Add support for key annotations to remote hyp
2910e333a runtime:  Use static resource in remote hypervisor
26d56678a config: Add initial remote hypervisor config
ad63439a3 runtime: Update the remote hypervisor config
50e0d43da runtime: Support privileged containers in peer pod VM
57d4dd8e5 runtime: Support the remote hypervisor type
8ac9a2209 runtime: Add hypervisor proto to support peer pod VMs
ee5589782 fmt: refactor in pci & balloon
baf3db9e6 Dragonball: add PCI bus and PCI interrupt support in mptable Spec
c305634b4 dragonball: Uniform the spelling of Virtio
c489f1f50 kata-deploy: Set a default value for ALLOWED_HYPERVISOR_ANNOTATIONS
ba632ba82 runitme-rs: kata with multi-containers sharing one direct volume
d7594d830 runtime-rs: correct the path from cid to device_id.
afec54799 libs: fixes dereferenced reference
c57df607a libs: fixes comparison to empty slice
c77e990c3 tests: Enable tests for StratoVirt hypervisor
14d8790d8 kata-deploy: Add StratoVirt support to deploy process
9542211e7 configuration: add configuration for StratoVirt hypervisor.
561c85be5 build: Makefile for StratoVirt hypervisor
26966c846 virtcontainers: Add StratoVirt as a supported hypervisor
0c7aa1f30 gha: Set nightly test for s390x to 5 UTC
ffe1ea52c tests|gha: add containerd and k8s tests for s390x
9d8eb298c metrics: Add iperf udp information to README
9cc6908b0 stability: Update stressng to run on the gha
4b7854b66 stability: Add missing dependencies
79177bb9c tests: Enable stressng scalability test
8959e3ca0 gha: Keep kata tarballs for 15 days
84b561873 tests|gha: add internal nightly tests for s390x
49c2e6e23 dragonball: Remove vhost-net dependency on virtio-net
bfd1ce30e kernel: Fix vsock packets drop when the vsock driver starts
849253e55 tests: Add a simple test to check the VMM vcpu allocation
5e9cf7593 vc: utils: Rename CalculateMilliCPUs() to CalculateCPUsF()
e477ed0e8 runtime: Improve vCPU allocation for the VMMs
b0157ad73 runtime: confidential: Do not set the max_vcpu to cpu
481486c6d gha: Remove docker and nerdctl tests from CI
b481d396f gha: Move docker / nerdctl content to the  basic-ci-amd64 file
3c735c236 ci: tracing: Adapt to basic-ci-amd64.yaml
ee17fe9d2 Revert "gha: ci: Revert tracing test PR to unbreak CI"
0ead018d0 utils: kata-manager: Add Docker details to list output
be3044fd0 utils: kata-manager: Add option to list versions
9969f5a94 utils: kata-manager: Make test container name more unique
436d7d127 utils: kata-manager: Improve usage message
1625a5ce4 utils: kata-manager: Improve version check
28e7b3467 metrics: improving stop and remove running containers
7f666f783 runtime-rs: ch: Fix TDX
d1deaf053 dragonball: Minor changes for a comment from Bian
e4f83e27c dragonball: vhost-net set_offload with acked features
6cd572dbb dragonball: Minor changes for Chao's comments
dcdf3c655 runtime-rs: Supply missing fields of NetworkConfig
58e9709c1 dragonball: Changes for ZizhengBian's comments
8ea87405e runtime-rs: Remove virtio config from Backend
ad66378bf runtime-rs: Move Dragonball stuff out of device drivers
3e0614cdf dragonball: Minor changes to comments
a047331a3 runtime-rs: Network config distinguishes backends
920337183 dragonball: Introduce vhost-net device
bc49c553e docs: add agent policy documentation
c72a27e21 utils: kata-manager: Ensure only one download URL
839f6c3d4 utils: kata-manager: Improve info messages
b27b4ce10 doc: No longer release the test repository
af2d897fb doc: Release now uses the official GitHub CLI
2af9419fa doc: No longer run kata-deploy test when releasing
5d10aed9b kata-manager: Make containerd_config a global var
66d1b2c17 kata-manager: Add support for docker installation
0352f1e02 kata-manager: Allow passing a specific tool to test_installation
afb002c25 runtime-rs: fix a typo in shm
78df1bb85 agent: update AGENT_THREADS metrics value
1a81989d2 tests: k8s: Use the "ALLOWED_HYPERVISOR_ANNOTATIONS"
023c4a17c kata-deploy: Allow users to set hypervisor annotations
455b7bf77 gha: k3s: Avoid unnecessary escape
e7890ee8f gha: Fix regex used to get kubectl version from the k3s version
071667f1c runtime: clh: Re-generate the client code
d1163141b versions: Upgrade to Cloud Hypervisor v36.0
acd9057c7 runtime: Fix TestCheckHostIsVMContainerCapable unstablity issue
c075fa681 tests: Add test with nerdctl to verify macvlan support
07db673eb tests: Add test with nerdctl to verify ipvlan support
a6272733e network: Fix network hotplug for ipvlan and macvlan endpoints.
a49bc6837 runtime-rs: Update status for pause and resume
023d8dc01 agent: Changes according to Pan's comments
136fb7622 tests: Add a integrated test for device cgroup
b5f3a8cb3 agent: Fix container launching failure with systemd cgroup
647782519 agent: Minor changes according to Zhou's comments
cec804474 agent: Make devcg_info optional for LinuxContainer::new()
ef4c3844a agent: Restrict device access at upper node of container's cgroup
59d0d4caf runtime-rs: ch: Simplify VSOCK error handling
bdb83f828 runtime-rs: ch: Remove unused function
5ef691528 tests: fixes permission denied when running test
dd530ba8e tests: fixes AMD errors
7641c19f7 runtime: bump containerd for gogo deprecation
16fa2c39e protocols: replace gogo/types.Empty and Any
c61f4a859 protocols: remove unused fieldpath option
c87bc60ea protocols: removing unused mappings
c5d845b30 agent: updating Cargo.lock files
5d88c78a6 protocols: generating agent.pb.go
036b7787d runtime-rs: Use PCI path from hypervisor for vfio devices
c3ce6a1d1 runtime-rs: Provide PCI path to the agent for virtio-block
a2bbbad71 runtime-rs: change hypervisor add_device trait to return device copy
8b4fc847d kata-manager: Accept only "lts" or "active" as containerd versions
37233622d kata-manager: Ensure we run apt-get update before apt-get install
994615ca2 gha: stale: Allow manually triggering it
6abcf0361 gha: stale: Fix typo action -> actions
fee97e219 docs: Fix Dragonball link
437db1591 kata-manager: Fix Mulit-Arch deployment for containerd
abec28705 gha: Add workflow to close stale PRs
d20b7381f release: Drop obsolete comment in workflow file
6236fa461 release: Drop build_hub helper
bc4c66caa release: Migrate tag_repos.sh to GitHub CLI
e331102ba release: Migrate update-repository-version.sh to GitHub CLI
b83a7149e release: Introduce helper to get GitHub CLI
ceeabe371 release: Allow to test release scripts with an alternate repo
58b4d1a26 cargo: Agent cargo.lock updated
0608e20a0 docs: Fix broken links
4ad2cfe0c runtime-rs: Log system enhancement
a0746c8d7 agent: Skip flaky create_tmpfs on s390x
f53f86884 network: Fix network attach for ipvlan and macvlan
c232869af metrics: removes double-quotes in checkemtrics when parsing results
c42a2f2ed metrics: increase the number of attempts to stop kata
1626253d9 metrics: FIO ci test enablement
873386a34 metrics: update iodepth and job size fio parameters to improve workload
ae3ea1421 utils: kata-manager: Fix containerd version check
346f19553 utils: kata-manager: Fix whitespace
2ac7ac1dd utils: kata-manager: Fix "Cannot determine download URL" issue
59bd53482 utils: kata-manager: Lint fixes
2f533c300 dragonball: add tracing feature for dragonball
d707fa2c0 kata-runtime/kata-ctl: Add security details to output
da77b1944 dragonball: output legacy device metrics to runtime
65213e9fb dragonball: unify the metric interface of legacy device
a3b003c34 agent: support bind mounts between containers
0ce0abffa tests/git-helper: cancel any previous rebase left halfway
f99de4d5a runtime-rs: Make default kernel params as empty
a81301278 runtime-rs: Add default configuration file for clouf-hypervisor
c20aadd7a gha: add dependencies for spell checker
d3250dff3 kata-manager: Add clh config to containerd config file
dce365d5b dragonball: add conditional compilation for BalloonDeviceMetrics
3819f0ee6 dragonball: output balloon device metrics to runtime
09d46450f dragonball: add metrics support for balloon device
f9c9d8f64 runtime: QemuVirt: hotadd virtio-mem dev to pcie root port
ef18c9550 runtime:qemuvirt: hotadd net dev to pcie root port
f1aec98f9 qemu/virt: use pcie_root_port to do device hotplug for virt
28a41e1d1 runtime: add a new API for Network interface
7d7c25c1d runtime-rs: fix a typo in device manager
2d0518cbe metrics: Add parallel udp iperf3 benchmark
</details>


fcd005774 tools: avoid rootfs-image build "ln -s" error
05c4c8055 runtime-rs: Configure argument replacement for QEMU in Makefile
27cb30d8c runtime-rs: Adjust configuration template for runtime-rs
462afcf82 runtime-rs: Copy configuration for QEMU from runtime
f139c7dc6 tests: k8s: k8s-copy-file auto-generated policy
1179306af tests: k8s: additional policy testing utilities
9a780aa98 genpolicy: improve logging from ExecProcessRequest
dab567bdf genpolicy: add easy way to allow CloseStdinRequest
8401adb11 genpolicy: update default values
ff1ace1c7 docs: Remove jenkins reference in kernel documentation
97fbf360c gha: Cleanup nydus snapshotter by the daemonset
43b04fd0c gha: Deploy nydus snapshotter by the daemonset
0b508f301 tests:k8s: make add_kernel_initrd_anotations function generic
a43edd0c3 rootfs: Install pause image into rootfs
42ef6bdca osbuilder:rootfs: support to unpack pause image to rootfs
53183cba3 workflow: Enable to build pause image in ci
70a84eca9 packaging: allow to pull and unpack pause image
3e383674f runtime: fix creation of SEV confidential container on SNP enabled host.
6346e04cf runtime-rs: fix handling of TTRCP_ADDRESS
f0256fded runtime-rs: remove validation of shim v2 -address value
34c47e08b runtime-rs: fix assert error in test in `make check`
