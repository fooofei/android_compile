[ 35% 12598/35754] Building with Jack: out/target/common/obj/JAVA_LIBRARIES/core-all_intermediates/with-local/classes.dex
FAILED: /bin/bash out/target/common/obj/JAVA_LIBRARIES/core-all_intermediates/with-local/classes.dex.rsp
Out of memory error (version 1.2-rc4 'Carnac' (298900 f95d7bdecfceb327f9d201a1348397ed8a843843 by android-jack-team@google.com)).
Java heap space.
Try increasing heap size with java option '-Xmx<size>'.
Warning: This may have produced partial or corrupted output.
[ 35% 12598/35754] build out/target/common/obj/JAVA_LIBRARIES/sdk_v9_intermediates/classes.jack
ninja: build stopped: subcommand failed.
build/core/ninja.mk:148: recipe for target 'ninja_wrapper' failed
make: *** [ninja_wrapper] Error 1




http://stackoverflow.com/questions/34940793/increasing-heap-size-while-building-the-android-source-code-on-ubuntu-15-10