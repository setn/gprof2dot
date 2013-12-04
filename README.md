gprof2dot
=========

Clone of jrfonseca's Gprof2Dot with Jruby profiling output support added by setn.

First create an output file from the Jruby profiler. See https://github.com/jruby/jruby/wiki/Profiling-jruby . Specificially use the GraphProfilePrinter output format.

Then run this gprof2dot with the JRuby format (-f jruby).

./gprof2dot -f jruby jruby.graph_format_profiling.out | dot -Tpng > profiling.png
