# Release 532567bfe9f28db48f4c0059ebddd9ef50ab631e

## kata-containers Changes
**FIXME - message this section by hand to produce a summary please**
### Shortlog
 236c2c765 tests: cri-o: Update critools version to 1.29
 344e0580c tests: cri-o: Use packages from pkgs.k8s.io
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
