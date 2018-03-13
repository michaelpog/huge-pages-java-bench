# huge-pages-java-bench
Benchmark that tests that transparent huge pages make any difference

Run baseline:
java -jar microbenchmarks.jar

Run with huge transparent pages:
java -XX:+UseTransparentHugePages -XX:+AlwaysPreTouch -jar microbenchmarks.jar

Run with profiler:
java -XX:+UseTransparentHugePages -XX:+AlwaysPreTouch -jar microbenchmarks.jar -prof  stack

Check what profilers are available:
java -XX:+UseTransparentHugePages -XX:+AlwaysPreTouch -jar microbenchmarks.jar -lprof
