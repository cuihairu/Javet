===================
Release Notes 3.0.x
===================

3.0.3 V8 v12.1
--------------

* Upgraded V8 to ``v12.1.285.26`` (2024-01-17)
* Upgraded Node.js to ``v20.11.0`` `(2024-01-09) <https://github.com/nodejs/node/blob/main/doc/changelogs/CHANGELOG_V20.md#20.11.0>`_
* Restore the reference lock
* Downgraded to Ubuntu 20.04 for better compatibility
* Fixed a slight memory leak in closing the V8 runtime
* Fixed a memory leak in dynamic proxy and dynamic object
* Applied a temporary `patch <https://github.com/caoccao/Javet/issues/290>`_ to V8 to avoid crashes on few Linux distributions in VM
* Added ``kNoStdioInitialization`` and ``kNoDefaultSignalHandling`` to Node.js initialization
* Improved performance of ``BaseJavetConsoleInterceptor``
* Added ``JavetJVMInterceptor``
* Added ``createSnapshot()`` to ``V8Runtime``
* Added ``isCreateSnapshotEnabled()``, ``setCreateSnapshotEnabled()``, ``getSnapshotBlob()``, ``setSnapshotBlob()`` to ``RuntimeOptions``
* Added ``RuntimeCreateSnapshotDisabled``, ``RuntimeCreateSnapshotBlocked`` to ``JavetError``
* Added ``isProxyListEnabled()``, ``setProxyListEnabled()`` to ``JavetConverterConfig``
* Added ``ArrayUtils``, ``CollectionUtils``
* Fixed ``CDTShell``

3.0.2 V8 v12.0
--------------

* Upgraded V8 to ``v12.0.267.8`` (2023-11-21)
* Upgraded Node.js to ``v20.10.0`` `(2023-11-22) <https://github.com/nodejs/node/blob/main/doc/changelogs/CHANGELOG_V20.md#20.10.0>`_
* Fixed Linux arm64 build addressing the changes in V8 v12

3.0.1 V8 v11.9
--------------

* Upgraded V8 to ``v11.9.169.6`` (2023-10-25)
* Upgraded Node.js to ``v20.9.0`` `(2023-10-24) <https://github.com/nodejs/node/blob/main/doc/changelogs/CHANGELOG_V20.md#20.9.0>`_
* Upgraded to Ubuntu 22.04
* Upgraded GCC to v11 on Linux
* Turned on a few compiler options for performance
* Added ``isSourceTextModule()``, ``isSyntheticModule()`` to ``V8Module``
* Added ``createV8Module()`` to ``V8Runtime``
* Added ``freeze()`` to ``V8ValueBuiltInObject``
* Added ``JavetBuiltInModuleResolver``

3.0.0 V8 v11.8
--------------

* Upgraded V8 to ``v11.8.172.15`` (2023-10-09)
* Upgraded Node.js to ``v20.8.0`` `(2023-09-28) <https://github.com/nodejs/node/blob/main/doc/changelogs/CHANGELOG_V20.md#20.8.0>`_
* Upgraded GCC to v10 on Linux
* Supported Linux arm64
* Fixed a contention issue in closing the reference
