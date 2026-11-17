# Benchmark snapshot

2026-11-17T12:13:55.074Z → 2026-11-17T12:25:41.136Z

**passed** · full · observed graphs · CellX standard

v24.22.2 · AMD EPYC 9V74 80-Core Processor · linux x64

578 measurements; 0 failed suites. Times are milliseconds. Each framework/suite runs in a fresh process; values are the minimum of 3 samples. Explicit GC is outside timing. Raw samples are in the adjacent JSON file. See the repository README for workload definitions and limitations.

## Comparison by workload family

Geometric mean of each case's time divided by the fastest engine on that case. Lower is better; 1× means fastest on every case in that family. Cases have equal weight within a family. There is no overall score. Small CellX timings are particularly sensitive to noise.

| Engine | kairo | mol | s | dynamic | cellx |
| --- | ---: | ---: | ---: | ---: | ---: |
| alien-signals | 1.11× | 1.25× | 1.15× | 1.32× | 1.21× |
| @angular/signals | 3.48× | 1.29× | 3.53× | 4.03× | 2.70× |
| MobX | 4.57× | 1.30× | 4.04× | 3.80× | 3.86× |
| $mol_wire | 4.50× | 1.00× | 4.74× | 2.80× | 2.93× |
| Oby | 2.45× | 1.52× | 4.75× | 2.88× | 2.92× |
| Pota | 3.56× | 1.52× | 3.97× | 3.19× | 1.51× |
| reflex-quant | 1.01× | 1.23× | 1.03× | 1.00× | 1.06× |
| x-reactivity | 5.43× | 1.57× | 4.36× | 4.80× | 5.34× |
| Preact Signals | 1.31× | 1.24× | 1.52× | 1.82× | 1.56× |
| TC39 Signals Polyfill | 7.00× | 1.35× | 4.39× | 14.61× | 3.16× |
| SolidJS | 4.77× | 1.53× | 3.89× | 5.70× | 2.20× |
| Svelte v5 | 5.19× | 1.34× | 3.79× | 26.03× | 42.00× |
| @amadeus-it-group/tansu | 3.26× | 1.29× | 3.56× | 2.63× | 2.60× |
| @tldraw/state | 4.35× | 1.33× | 3.24× | 7.34× | 3.19× |
| uSignal | 3.79× | 1.75× | 3.01× | 3.40× | 2.07× |
| @vue/reactivity | 2.23× | 1.26× | 1.86× | 2.45× | 2.63× |
| @pravosleva/reactive-engine | 2.04× | 1.27× | 3.85× | 1.84× | 2.03× |

## Packages

| Package | Version |
| --- | --- |
| alien-signals | 3.2.1 |
| @angular/core | 22.2.6 |
| mobx | 7.1.7 |
| mol_wire_lib | 1.0.1845 |
| oby | 15.1.2 |
| pota | 0.22.235 |
| reflex-quant | 1.2.0 |
| @solidjs/signals | 2.0.0-rc.22 |
| @preact/signals-core | 1.14.5 |
| signal-polyfill | 0.2.2 |
| solid-js | 1.9.19 |
| svelte | 5.57.3 |
| @amadeus-it-group/tansu | 2.0.0 |
| @tldraw/state | 5.6.0 |
| usignal | 0.10.0 |
| @vue/reactivity | 3.5.45 |
| @pravosleva/reactive-engine | 3.0.0 |

## Measurements

| Framework | Suite | Test | ms |
| --- | --- | --- | ---: |
| alien-signals | kairo | avoidablePropagation | 95.3891 |
| alien-signals | kairo | broadPropagation | 233.7072 |
| alien-signals | kairo | deepPropagation | 70.7146 |
| alien-signals | kairo | diamond | 129.4377 |
| alien-signals | kairo | mux | 223.0087 |
| alien-signals | kairo | repeatedObservers | 14.5474 |
| alien-signals | kairo | triangle | 49.1169 |
| alien-signals | kairo | unstable | 47.4931 |
| alien-signals | mol | molBench | 518.4617 |
| alien-signals | s | createDataSignals | 6.1955 |
| alien-signals | s | createComputations0to1 | 4.0176 |
| alien-signals | s | createComputations1to1 | 11.1879 |
| alien-signals | s | createComputations2to1 | 9.6422 |
| alien-signals | s | createComputations4to1 | 8.9234 |
| alien-signals | s | createComputations1000to1 | 7.7849 |
| alien-signals | s | createComputations1to2 | 8.8466 |
| alien-signals | s | createComputations1to4 | 7.6926 |
| alien-signals | s | createComputations1to8 | 6.9109 |
| alien-signals | s | createComputations1to1000 | 6.8102 |
| alien-signals | s | updateComputations1to1 | 23.1641 |
| alien-signals | s | updateComputations2to1 | 14.6455 |
| alien-signals | s | updateComputations4to1 | 9.2665 |
| alien-signals | s | updateComputations1000to1 | 4.1380 |
| alien-signals | s | updateComputations1to2 | 15.6222 |
| alien-signals | s | updateComputations1to4 | 13.4543 |
| alien-signals | s | updateComputations1to1000 | 12.3923 |
| alien-signals | dynamic | 10x5 - 2 sources - read 20% (simple component) | 176.0352 |
| alien-signals | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 155.4741 |
| alien-signals | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 251.0138 |
| alien-signals | dynamic | 1000x5 - 25 sources (wide dense) | 488.5729 |
| alien-signals | dynamic | 5x500 - 3 sources (deep) | 130.1960 |
| alien-signals | cellx | cellx10 | 0.0500 |
| alien-signals | cellx | cellx20 | 0.0712 |
| alien-signals | cellx | cellx30 | 0.0744 |
| @angular/signals | kairo | avoidablePropagation | 332.0811 |
| @angular/signals | kairo | broadPropagation | 696.2291 |
| @angular/signals | kairo | deepPropagation | 227.7091 |
| @angular/signals | kairo | diamond | 431.4929 |
| @angular/signals | kairo | mux | 503.6312 |
| @angular/signals | kairo | repeatedObservers | 55.7507 |
| @angular/signals | kairo | triangle | 162.4053 |
| @angular/signals | kairo | unstable | 136.4700 |
| @angular/signals | mol | molBench | 533.8906 |
| @angular/signals | s | createDataSignals | 61.8374 |
| @angular/signals | s | createComputations0to1 | 10.5000 |
| @angular/signals | s | createComputations1to1 | 72.1112 |
| @angular/signals | s | createComputations2to1 | 67.9597 |
| @angular/signals | s | createComputations4to1 | 63.1823 |
| @angular/signals | s | createComputations1000to1 | 60.5539 |
| @angular/signals | s | createComputations1to2 | 29.6869 |
| @angular/signals | s | createComputations1to4 | 25.0139 |
| @angular/signals | s | createComputations1to8 | 17.9483 |
| @angular/signals | s | createComputations1to1000 | 15.1567 |
| @angular/signals | s | updateComputations1to1 | 33.9394 |
| @angular/signals | s | updateComputations2to1 | 22.5982 |
| @angular/signals | s | updateComputations4to1 | 13.0886 |
| @angular/signals | s | updateComputations1000to1 | 5.9662 |
| @angular/signals | s | updateComputations1to2 | 33.2282 |
| @angular/signals | s | updateComputations1to4 | 29.2187 |
| @angular/signals | s | updateComputations1to1000 | 28.6302 |
| @angular/signals | dynamic | 10x5 - 2 sources - read 20% (simple component) | 729.3706 |
| @angular/signals | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 417.4780 |
| @angular/signals | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 822.1058 |
| @angular/signals | dynamic | 1000x5 - 25 sources (wide dense) | 1320.2442 |
| @angular/signals | dynamic | 5x500 - 3 sources (deep) | 357.7117 |
| @angular/signals | cellx | cellx10 | 0.1154 |
| @angular/signals | cellx | cellx20 | 0.1418 |
| @angular/signals | cellx | cellx30 | 0.1817 |
| MobX | kairo | avoidablePropagation | 465.0659 |
| MobX | kairo | broadPropagation | 1131.7129 |
| MobX | kairo | deepPropagation | 478.2073 |
| MobX | kairo | diamond | 636.1560 |
| MobX | kairo | mux | 527.6938 |
| MobX | kairo | repeatedObservers | 50.6340 |
| MobX | kairo | triangle | 218.0114 |
| MobX | kairo | unstable | 136.0683 |
| MobX | mol | molBench | 540.0356 |
| MobX | s | createDataSignals | 9.8259 |
| MobX | s | createComputations0to1 | 22.1953 |
| MobX | s | createComputations1to1 | 68.9731 |
| MobX | s | createComputations2to1 | 54.4099 |
| MobX | s | createComputations4to1 | 26.7490 |
| MobX | s | createComputations1000to1 | 12.3466 |
| MobX | s | createComputations1to2 | 61.4371 |
| MobX | s | createComputations1to4 | 49.2678 |
| MobX | s | createComputations1to8 | 48.8396 |
| MobX | s | createComputations1to1000 | 49.5791 |
| MobX | s | updateComputations1to1 | 56.5224 |
| MobX | s | updateComputations2to1 | 32.0554 |
| MobX | s | updateComputations4to1 | 19.2395 |
| MobX | s | updateComputations1000to1 | 6.5394 |
| MobX | s | updateComputations1to2 | 46.8157 |
| MobX | s | updateComputations1to4 | 44.6977 |
| MobX | s | updateComputations1to1000 | 42.3626 |
| MobX | dynamic | 10x5 - 2 sources - read 20% (simple component) | 766.2164 |
| MobX | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 452.4073 |
| MobX | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 682.2733 |
| MobX | dynamic | 1000x5 - 25 sources (wide dense) | 935.9349 |
| MobX | dynamic | 5x500 - 3 sources (deep) | 397.1197 |
| MobX | cellx | cellx10 | 0.1387 |
| MobX | cellx | cellx20 | 0.2164 |
| MobX | cellx | cellx30 | 0.2897 |
| $mol_wire | kairo | avoidablePropagation | 336.6249 |
| $mol_wire | kairo | broadPropagation | 983.6454 |
| $mol_wire | kairo | deepPropagation | 301.0865 |
| $mol_wire | kairo | diamond | 463.3626 |
| $mol_wire | kairo | mux | 641.6946 |
| $mol_wire | kairo | repeatedObservers | 88.7899 |
| $mol_wire | kairo | triangle | 156.0811 |
| $mol_wire | kairo | unstable | 271.5483 |
| $mol_wire | mol | molBench | 415.4007 |
| $mol_wire | s | createDataSignals | 23.9466 |
| $mol_wire | s | createComputations0to1 | 15.5826 |
| $mol_wire | s | createComputations1to1 | 114.5369 |
| $mol_wire | s | createComputations2to1 | 40.9679 |
| $mol_wire | s | createComputations4to1 | 37.9845 |
| $mol_wire | s | createComputations1000to1 | 28.3158 |
| $mol_wire | s | createComputations1to2 | 66.9738 |
| $mol_wire | s | createComputations1to4 | 29.5468 |
| $mol_wire | s | createComputations1to8 | 25.2587 |
| $mol_wire | s | createComputations1to1000 | 24.0335 |
| $mol_wire | s | updateComputations1to1 | 85.0854 |
| $mol_wire | s | updateComputations2to1 | 46.9607 |
| $mol_wire | s | updateComputations4to1 | 30.9112 |
| $mol_wire | s | updateComputations1000to1 | 9.4960 |
| $mol_wire | s | updateComputations1to2 | 68.6678 |
| $mol_wire | s | updateComputations1to4 | 58.4916 |
| $mol_wire | s | updateComputations1to1000 | 57.7890 |
| $mol_wire | dynamic | 10x5 - 2 sources - read 20% (simple component) | 544.1105 |
| $mol_wire | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 316.4379 |
| $mol_wire | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 558.0413 |
| $mol_wire | dynamic | 1000x5 - 25 sources (wide dense) | 695.7248 |
| $mol_wire | dynamic | 5x500 - 3 sources (deep) | 285.4344 |
| $mol_wire | cellx | cellx10 | 0.1535 |
| $mol_wire | cellx | cellx20 | 0.1384 |
| $mol_wire | cellx | cellx30 | 0.1784 |
| Oby | kairo | avoidablePropagation | 206.7629 |
| Oby | kairo | broadPropagation | 520.4356 |
| Oby | kairo | deepPropagation | 242.0424 |
| Oby | kairo | diamond | 311.0189 |
| Oby | kairo | mux | 346.5356 |
| Oby | kairo | repeatedObservers | 37.2008 |
| Oby | kairo | triangle | 119.3812 |
| Oby | kairo | unstable | 68.7987 |
| Oby | mol | molBench | 629.7882 |
| Oby | s | createDataSignals | 13.0956 |
| Oby | s | createComputations0to1 | 39.3412 |
| Oby | s | createComputations1to1 | 105.8705 |
| Oby | s | createComputations2to1 | 74.9199 |
| Oby | s | createComputations4to1 | 50.4560 |
| Oby | s | createComputations1000to1 | 16.2008 |
| Oby | s | createComputations1to2 | 82.2637 |
| Oby | s | createComputations1to4 | 65.7619 |
| Oby | s | createComputations1to8 | 71.0870 |
| Oby | s | createComputations1to1000 | 62.8144 |
| Oby | s | updateComputations1to1 | 38.1772 |
| Oby | s | updateComputations2to1 | 24.9491 |
| Oby | s | updateComputations4to1 | 16.2588 |
| Oby | s | updateComputations1000to1 | 14.0850 |
| Oby | s | updateComputations1to2 | 34.4362 |
| Oby | s | updateComputations1to4 | 31.5816 |
| Oby | s | updateComputations1to1000 | 32.9789 |
| Oby | dynamic | 10x5 - 2 sources - read 20% (simple component) | 470.8002 |
| Oby | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 358.3907 |
| Oby | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 576.5920 |
| Oby | dynamic | 1000x5 - 25 sources (wide dense) | 826.3324 |
| Oby | dynamic | 5x500 - 3 sources (deep) | 275.4767 |
| Oby | cellx | cellx10 | 0.1430 |
| Oby | cellx | cellx20 | 0.1856 |
| Oby | cellx | cellx30 | 0.1425 |
| Pota | kairo | avoidablePropagation | 447.2486 |
| Pota | kairo | broadPropagation | 625.2425 |
| Pota | kairo | deepPropagation | 272.2122 |
| Pota | kairo | diamond | 406.1440 |
| Pota | kairo | mux | 385.8708 |
| Pota | kairo | repeatedObservers | 86.9508 |
| Pota | kairo | triangle | 134.4272 |
| Pota | kairo | unstable | 123.1283 |
| Pota | mol | molBench | 632.5971 |
| Pota | s | createDataSignals | 13.0540 |
| Pota | s | createComputations0to1 | 11.3003 |
| Pota | s | createComputations1to1 | 69.3509 |
| Pota | s | createComputations2to1 | 64.7149 |
| Pota | s | createComputations4to1 | 64.2398 |
| Pota | s | createComputations1000to1 | 15.1622 |
| Pota | s | createComputations1to2 | 70.7253 |
| Pota | s | createComputations1to4 | 19.5288 |
| Pota | s | createComputations1to8 | 19.1936 |
| Pota | s | createComputations1to1000 | 14.4739 |
| Pota | s | updateComputations1to1 | 81.8063 |
| Pota | s | updateComputations2to1 | 48.0073 |
| Pota | s | updateComputations4to1 | 29.9468 |
| Pota | s | updateComputations1000to1 | 11.2816 |
| Pota | s | updateComputations1to2 | 57.6914 |
| Pota | s | updateComputations1to4 | 44.9954 |
| Pota | s | updateComputations1to1000 | 36.2263 |
| Pota | dynamic | 10x5 - 2 sources - read 20% (simple component) | 756.1943 |
| Pota | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 377.6238 |
| Pota | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 477.2174 |
| Pota | dynamic | 1000x5 - 25 sources (wide dense) | 831.0741 |
| Pota | dynamic | 5x500 - 3 sources (deep) | 321.4190 |
| Pota | cellx | cellx10 | 0.0953 |
| Pota | cellx | cellx20 | 0.0934 |
| Pota | cellx | cellx30 | 0.0591 |
| reflex-quant | kairo | avoidablePropagation | 93.3470 |
| reflex-quant | kairo | broadPropagation | 188.8129 |
| reflex-quant | kairo | deepPropagation | 77.7161 |
| reflex-quant | kairo | diamond | 106.9674 |
| reflex-quant | kairo | mux | 213.0638 |
| reflex-quant | kairo | repeatedObservers | 14.8163 |
| reflex-quant | kairo | triangle | 42.3207 |
| reflex-quant | kairo | unstable | 37.9745 |
| reflex-quant | mol | molBench | 512.0969 |
| reflex-quant | s | createDataSignals | 6.0796 |
| reflex-quant | s | createComputations0to1 | 4.4231 |
| reflex-quant | s | createComputations1to1 | 12.5443 |
| reflex-quant | s | createComputations2to1 | 10.2337 |
| reflex-quant | s | createComputations4to1 | 9.2623 |
| reflex-quant | s | createComputations1000to1 | 8.0221 |
| reflex-quant | s | createComputations1to2 | 8.8785 |
| reflex-quant | s | createComputations1to4 | 7.2729 |
| reflex-quant | s | createComputations1to8 | 6.3748 |
| reflex-quant | s | createComputations1to1000 | 6.2338 |
| reflex-quant | s | updateComputations1to1 | 17.9861 |
| reflex-quant | s | updateComputations2to1 | 10.9306 |
| reflex-quant | s | updateComputations4to1 | 7.1793 |
| reflex-quant | s | updateComputations1000to1 | 2.2756 |
| reflex-quant | s | updateComputations1to2 | 12.6044 |
| reflex-quant | s | updateComputations1to4 | 11.3789 |
| reflex-quant | s | updateComputations1to1000 | 10.9502 |
| reflex-quant | dynamic | 10x5 - 2 sources - read 20% (simple component) | 164.0100 |
| reflex-quant | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 123.4717 |
| reflex-quant | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 174.1088 |
| reflex-quant | dynamic | 1000x5 - 25 sources (wide dense) | 278.2414 |
| reflex-quant | dynamic | 5x500 - 3 sources (deep) | 112.9570 |
| reflex-quant | cellx | cellx10 | 0.0566 |
| reflex-quant | cellx | cellx20 | 0.0512 |
| reflex-quant | cellx | cellx30 | 0.0618 |
| x-reactivity | kairo | avoidablePropagation | 553.0679 |
| x-reactivity | kairo | broadPropagation | 1025.3439 |
| x-reactivity | kairo | deepPropagation | 344.5871 |
| x-reactivity | kairo | diamond | 782.8493 |
| x-reactivity | kairo | mux | 387.4900 |
| x-reactivity | kairo | repeatedObservers | 129.4681 |
| x-reactivity | kairo | triangle | 299.2163 |
| x-reactivity | kairo | unstable | 219.1795 |
| x-reactivity | mol | molBench | 653.8118 |
| x-reactivity | s | createDataSignals | 12.5673 |
| x-reactivity | s | createComputations0to1 | 10.9662 |
| x-reactivity | s | createComputations1to1 | 74.8263 |
| x-reactivity | s | createComputations2to1 | 62.2650 |
| x-reactivity | s | createComputations4to1 | 18.7033 |
| x-reactivity | s | createComputations1000to1 | 13.7974 |
| x-reactivity | s | createComputations1to2 | 28.4763 |
| x-reactivity | s | createComputations1to4 | 17.9642 |
| x-reactivity | s | createComputations1to8 | 19.6135 |
| x-reactivity | s | createComputations1to1000 | 16.6670 |
| x-reactivity | s | updateComputations1to1 | 160.9096 |
| x-reactivity | s | updateComputations2to1 | 90.1692 |
| x-reactivity | s | updateComputations4to1 | 48.3790 |
| x-reactivity | s | updateComputations1000to1 | 13.4048 |
| x-reactivity | s | updateComputations1to2 | 118.7178 |
| x-reactivity | s | updateComputations1to4 | 82.6552 |
| x-reactivity | s | updateComputations1to1000 | 59.0272 |
| x-reactivity | dynamic | 10x5 - 2 sources - read 20% (simple component) | 1925.1886 |
| x-reactivity | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 483.0327 |
| x-reactivity | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 771.4090 |
| x-reactivity | dynamic | 1000x5 - 25 sources (wide dense) | 1138.7808 |
| x-reactivity | dynamic | 5x500 - 3 sources (deep) | 346.2243 |
| x-reactivity | cellx | cellx10 | 0.2381 |
| x-reactivity | cellx | cellx20 | 0.3017 |
| x-reactivity | cellx | cellx30 | 0.3209 |
| Preact Signals | kairo | avoidablePropagation | 120.4715 |
| Preact Signals | kairo | broadPropagation | 232.3712 |
| Preact Signals | kairo | deepPropagation | 98.4546 |
| Preact Signals | kairo | diamond | 176.3530 |
| Preact Signals | kairo | mux | 253.4811 |
| Preact Signals | kairo | repeatedObservers | 17.3099 |
| Preact Signals | kairo | triangle | 67.0727 |
| Preact Signals | kairo | unstable | 40.3876 |
| Preact Signals | mol | molBench | 516.9487 |
| Preact Signals | s | createDataSignals | 7.3235 |
| Preact Signals | s | createComputations0to1 | 7.9250 |
| Preact Signals | s | createComputations1to1 | 26.7706 |
| Preact Signals | s | createComputations2to1 | 10.2356 |
| Preact Signals | s | createComputations4to1 | 14.3286 |
| Preact Signals | s | createComputations1000to1 | 10.2264 |
| Preact Signals | s | createComputations1to2 | 14.4459 |
| Preact Signals | s | createComputations1to4 | 13.0170 |
| Preact Signals | s | createComputations1to8 | 13.2179 |
| Preact Signals | s | createComputations1to1000 | 5.3516 |
| Preact Signals | s | updateComputations1to1 | 24.5173 |
| Preact Signals | s | updateComputations2to1 | 16.2880 |
| Preact Signals | s | updateComputations4to1 | 11.2230 |
| Preact Signals | s | updateComputations1000to1 | 5.5001 |
| Preact Signals | s | updateComputations1to2 | 17.2060 |
| Preact Signals | s | updateComputations1to4 | 14.6418 |
| Preact Signals | s | updateComputations1to1000 | 12.6794 |
| Preact Signals | dynamic | 10x5 - 2 sources - read 20% (simple component) | 282.8949 |
| Preact Signals | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 223.7164 |
| Preact Signals | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 316.5999 |
| Preact Signals | dynamic | 1000x5 - 25 sources (wide dense) | 586.6034 |
| Preact Signals | dynamic | 5x500 - 3 sources (deep) | 190.5178 |
| Preact Signals | cellx | cellx10 | 0.0964 |
| Preact Signals | cellx | cellx20 | 0.0998 |
| Preact Signals | cellx | cellx30 | 0.0598 |
| TC39 Signals Polyfill | kairo | avoidablePropagation | 450.8698 |
| TC39 Signals Polyfill | kairo | broadPropagation | 1102.6591 |
| TC39 Signals Polyfill | kairo | deepPropagation | 355.3627 |
| TC39 Signals Polyfill | kairo | diamond | 691.2867 |
| TC39 Signals Polyfill | kairo | mux | 800.7125 |
| TC39 Signals Polyfill | kairo | repeatedObservers | 207.1226 |
| TC39 Signals Polyfill | kairo | triangle | 259.3083 |
| TC39 Signals Polyfill | kairo | unstable | 727.0411 |
| TC39 Signals Polyfill | mol | molBench | 561.1867 |
| TC39 Signals Polyfill | s | createDataSignals | 18.6702 |
| TC39 Signals Polyfill | s | createComputations0to1 | 28.3281 |
| TC39 Signals Polyfill | s | createComputations1to1 | 69.3133 |
| TC39 Signals Polyfill | s | createComputations2to1 | 43.3245 |
| TC39 Signals Polyfill | s | createComputations4to1 | 31.5997 |
| TC39 Signals Polyfill | s | createComputations1000to1 | 23.0522 |
| TC39 Signals Polyfill | s | createComputations1to2 | 52.6713 |
| TC39 Signals Polyfill | s | createComputations1to4 | 47.2897 |
| TC39 Signals Polyfill | s | createComputations1to8 | 45.8810 |
| TC39 Signals Polyfill | s | createComputations1to1000 | 38.2429 |
| TC39 Signals Polyfill | s | updateComputations1to1 | 55.9067 |
| TC39 Signals Polyfill | s | updateComputations2to1 | 34.9884 |
| TC39 Signals Polyfill | s | updateComputations4to1 | 23.4809 |
| TC39 Signals Polyfill | s | updateComputations1000to1 | 9.4747 |
| TC39 Signals Polyfill | s | updateComputations1to2 | 47.5267 |
| TC39 Signals Polyfill | s | updateComputations1to4 | 40.0241 |
| TC39 Signals Polyfill | s | updateComputations1to1000 | 40.5106 |
| TC39 Signals Polyfill | dynamic | 10x5 - 2 sources - read 20% (simple component) | 1882.5041 |
| TC39 Signals Polyfill | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 629.4120 |
| TC39 Signals Polyfill | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 13836.5742 |
| TC39 Signals Polyfill | dynamic | 1000x5 - 25 sources (wide dense) | 9417.3828 |
| TC39 Signals Polyfill | dynamic | 5x500 - 3 sources (deep) | 477.4108 |
| TC39 Signals Polyfill | cellx | cellx10 | 0.1348 |
| TC39 Signals Polyfill | cellx | cellx20 | 0.2065 |
| TC39 Signals Polyfill | cellx | cellx30 | 0.1721 |
| SolidJS | kairo | avoidablePropagation | 472.1639 |
| SolidJS | kairo | broadPropagation | 1001.9094 |
| SolidJS | kairo | deepPropagation | 418.3164 |
| SolidJS | kairo | diamond | 682.5636 |
| SolidJS | kairo | mux | 563.4575 |
| SolidJS | kairo | repeatedObservers | 85.0815 |
| SolidJS | kairo | triangle | 209.9044 |
| SolidJS | kairo | unstable | 130.0501 |
| SolidJS | mol | molBench | 633.7142 |
| SolidJS | s | createDataSignals | 9.3237 |
| SolidJS | s | createComputations0to1 | 9.9126 |
| SolidJS | s | createComputations1to1 | 67.0727 |
| SolidJS | s | createComputations2to1 | 61.8629 |
| SolidJS | s | createComputations4to1 | 41.9467 |
| SolidJS | s | createComputations1000to1 | 10.4840 |
| SolidJS | s | createComputations1to2 | 59.8135 |
| SolidJS | s | createComputations1to4 | 15.3648 |
| SolidJS | s | createComputations1to8 | 13.4653 |
| SolidJS | s | createComputations1to1000 | 12.6923 |
| SolidJS | s | updateComputations1to1 | 80.3760 |
| SolidJS | s | updateComputations2to1 | 57.1891 |
| SolidJS | s | updateComputations4to1 | 44.7947 |
| SolidJS | s | updateComputations1000to1 | 34.7070 |
| SolidJS | s | updateComputations1to2 | 52.5338 |
| SolidJS | s | updateComputations1to4 | 46.5189 |
| SolidJS | s | updateComputations1to1000 | 45.9462 |
| SolidJS | dynamic | 10x5 - 2 sources - read 20% (simple component) | 1904.0730 |
| SolidJS | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 651.6768 |
| SolidJS | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 812.3709 |
| SolidJS | dynamic | 1000x5 - 25 sources (wide dense) | 1358.4530 |
| SolidJS | dynamic | 5x500 - 3 sources (deep) | 487.8288 |
| SolidJS | cellx | cellx10 | 0.1114 |
| SolidJS | cellx | cellx20 | 0.1520 |
| SolidJS | cellx | cellx30 | 0.0949 |
| Svelte v5 | kairo | avoidablePropagation | 776.2882 |
| Svelte v5 | kairo | broadPropagation | 892.3651 |
| Svelte v5 | kairo | deepPropagation | 387.9007 |
| Svelte v5 | kairo | diamond | 804.3322 |
| Svelte v5 | kairo | mux | 359.2200 |
| Svelte v5 | kairo | repeatedObservers | 97.5711 |
| Svelte v5 | kairo | triangle | 262.9931 |
| Svelte v5 | kairo | unstable | 174.3855 |
| Svelte v5 | mol | molBench | 554.6582 |
| Svelte v5 | s | createDataSignals | 6.7850 |
| Svelte v5 | s | createComputations0to1 | 30.3331 |
| Svelte v5 | s | createComputations1to1 | 37.2426 |
| Svelte v5 | s | createComputations2to1 | 25.3562 |
| Svelte v5 | s | createComputations4to1 | 16.9841 |
| Svelte v5 | s | createComputations1000to1 | 7.6963 |
| Svelte v5 | s | createComputations1to2 | 29.6720 |
| Svelte v5 | s | createComputations1to4 | 25.1786 |
| Svelte v5 | s | createComputations1to8 | 23.8725 |
| Svelte v5 | s | createComputations1to1000 | 23.3515 |
| Svelte v5 | s | updateComputations1to1 | 203.9475 |
| Svelte v5 | s | updateComputations2to1 | 105.5639 |
| Svelte v5 | s | updateComputations4to1 | 55.6964 |
| Svelte v5 | s | updateComputations1000to1 | 5.0432 |
| Svelte v5 | s | updateComputations1to2 | 117.3173 |
| Svelte v5 | s | updateComputations1to4 | 71.0154 |
| Svelte v5 | s | updateComputations1to1000 | 25.3886 |
| Svelte v5 | dynamic | 10x5 - 2 sources - read 20% (simple component) | 993.6918 |
| Svelte v5 | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 21868.0449 |
| Svelte v5 | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 10561.9436 |
| Svelte v5 | dynamic | 1000x5 - 25 sources (wide dense) | 4993.0922 |
| Svelte v5 | dynamic | 5x500 - 3 sources (deep) | 1156.5906 |
| Svelte v5 | cellx | cellx10 | 0.2486 |
| Svelte v5 | cellx | cellx20 | 5.6800 |
| Svelte v5 | cellx | cellx30 | 7.9399 |
| @amadeus-it-group/tansu | kairo | avoidablePropagation | 297.8924 |
| @amadeus-it-group/tansu | kairo | broadPropagation | 667.8799 |
| @amadeus-it-group/tansu | kairo | deepPropagation | 231.5025 |
| @amadeus-it-group/tansu | kairo | diamond | 317.0007 |
| @amadeus-it-group/tansu | kairo | mux | 460.9810 |
| @amadeus-it-group/tansu | kairo | repeatedObservers | 58.7837 |
| @amadeus-it-group/tansu | kairo | triangle | 123.7781 |
| @amadeus-it-group/tansu | kairo | unstable | 172.4889 |
| @amadeus-it-group/tansu | mol | molBench | 537.7817 |
| @amadeus-it-group/tansu | s | createDataSignals | 13.1659 |
| @amadeus-it-group/tansu | s | createComputations0to1 | 16.0875 |
| @amadeus-it-group/tansu | s | createComputations1to1 | 67.3686 |
| @amadeus-it-group/tansu | s | createComputations2to1 | 42.1690 |
| @amadeus-it-group/tansu | s | createComputations4to1 | 22.5333 |
| @amadeus-it-group/tansu | s | createComputations1000to1 | 22.2707 |
| @amadeus-it-group/tansu | s | createComputations1to2 | 46.6943 |
| @amadeus-it-group/tansu | s | createComputations1to4 | 38.6562 |
| @amadeus-it-group/tansu | s | createComputations1to8 | 31.4344 |
| @amadeus-it-group/tansu | s | createComputations1to1000 | 34.0146 |
| @amadeus-it-group/tansu | s | updateComputations1to1 | 43.2692 |
| @amadeus-it-group/tansu | s | updateComputations2to1 | 27.2118 |
| @amadeus-it-group/tansu | s | updateComputations4to1 | 17.5142 |
| @amadeus-it-group/tansu | s | updateComputations1000to1 | 7.2553 |
| @amadeus-it-group/tansu | s | updateComputations1to2 | 40.4378 |
| @amadeus-it-group/tansu | s | updateComputations1to4 | 36.8828 |
| @amadeus-it-group/tansu | s | updateComputations1to1000 | 37.3039 |
| @amadeus-it-group/tansu | dynamic | 10x5 - 2 sources - read 20% (simple component) | 510.1492 |
| @amadeus-it-group/tansu | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 261.0684 |
| @amadeus-it-group/tansu | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 572.8239 |
| @amadeus-it-group/tansu | dynamic | 1000x5 - 25 sources (wide dense) | 667.2390 |
| @amadeus-it-group/tansu | dynamic | 5x500 - 3 sources (deep) | 272.5575 |
| @amadeus-it-group/tansu | cellx | cellx10 | 0.1740 |
| @amadeus-it-group/tansu | cellx | cellx20 | 0.1504 |
| @amadeus-it-group/tansu | cellx | cellx30 | 0.1022 |
| @tldraw/state | kairo | avoidablePropagation | 401.6793 |
| @tldraw/state | kairo | broadPropagation | 944.3262 |
| @tldraw/state | kairo | deepPropagation | 317.5327 |
| @tldraw/state | kairo | diamond | 542.8442 |
| @tldraw/state | kairo | mux | 577.9765 |
| @tldraw/state | kairo | repeatedObservers | 73.1716 |
| @tldraw/state | kairo | triangle | 239.7341 |
| @tldraw/state | kairo | unstable | 127.6581 |
| @tldraw/state | mol | molBench | 552.6527 |
| @tldraw/state | s | createDataSignals | 9.4156 |
| @tldraw/state | s | createComputations0to1 | 9.1055 |
| @tldraw/state | s | createComputations1to1 | 24.7953 |
| @tldraw/state | s | createComputations2to1 | 20.8319 |
| @tldraw/state | s | createComputations4to1 | 12.2567 |
| @tldraw/state | s | createComputations1000to1 | 17.5206 |
| @tldraw/state | s | createComputations1to2 | 26.3361 |
| @tldraw/state | s | createComputations1to4 | 21.1300 |
| @tldraw/state | s | createComputations1to8 | 19.2984 |
| @tldraw/state | s | createComputations1to1000 | 18.2727 |
| @tldraw/state | s | updateComputations1to1 | 78.0109 |
| @tldraw/state | s | updateComputations2to1 | 50.1594 |
| @tldraw/state | s | updateComputations4to1 | 36.2662 |
| @tldraw/state | s | updateComputations1000to1 | 18.9003 |
| @tldraw/state | s | updateComputations1to2 | 68.8004 |
| @tldraw/state | s | updateComputations1to4 | 58.4025 |
| @tldraw/state | s | updateComputations1to1000 | 47.2485 |
| @tldraw/state | dynamic | 10x5 - 2 sources - read 20% (simple component) | 806.0021 |
| @tldraw/state | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 423.6136 |
| @tldraw/state | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 4964.0880 |
| @tldraw/state | dynamic | 1000x5 - 25 sources (wide dense) | 3972.8658 |
| @tldraw/state | dynamic | 5x500 - 3 sources (deep) | 350.7612 |
| @tldraw/state | cellx | cellx10 | 0.1275 |
| @tldraw/state | cellx | cellx20 | 0.2266 |
| @tldraw/state | cellx | cellx30 | 0.1694 |
| uSignal | kairo | avoidablePropagation | 606.1288 |
| uSignal | kairo | broadPropagation | 885.4443 |
| uSignal | kairo | deepPropagation | 283.3382 |
| uSignal | kairo | diamond | 405.9484 |
| uSignal | kairo | mux | 672.5798 |
| uSignal | kairo | repeatedObservers | 54.8550 |
| uSignal | kairo | triangle | 159.2961 |
| uSignal | kairo | unstable | 77.6305 |
| uSignal | mol | molBench | 727.5129 |
| uSignal | s | createDataSignals | 10.0877 |
| uSignal | s | createComputations0to1 | 10.6129 |
| uSignal | s | createComputations1to1 | 56.8912 |
| uSignal | s | createComputations2to1 | 20.8588 |
| uSignal | s | createComputations4to1 | 16.8056 |
| uSignal | s | createComputations1000to1 | 15.0549 |
| uSignal | s | createComputations1to2 | 51.1398 |
| uSignal | s | createComputations1to4 | 32.3576 |
| uSignal | s | createComputations1to8 | 31.5746 |
| uSignal | s | createComputations1to1000 | 15.7123 |
| uSignal | s | updateComputations1to1 | 43.5361 |
| uSignal | s | updateComputations2to1 | 26.7463 |
| uSignal | s | updateComputations4to1 | 17.1203 |
| uSignal | s | updateComputations1000to1 | 11.0907 |
| uSignal | s | updateComputations1to2 | 37.3568 |
| uSignal | s | updateComputations1to4 | 33.4669 |
| uSignal | s | updateComputations1to1000 | 36.7770 |
| uSignal | dynamic | 10x5 - 2 sources - read 20% (simple component) | 513.8338 |
| uSignal | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 471.5353 |
| uSignal | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 496.5144 |
| uSignal | dynamic | 1000x5 - 25 sources (wide dense) | 1221.3815 |
| uSignal | dynamic | 5x500 - 3 sources (deep) | 342.6340 |
| uSignal | cellx | cellx10 | 0.1030 |
| uSignal | cellx | cellx20 | 0.1431 |
| uSignal | cellx | cellx30 | 0.0908 |
| @vue/reactivity | kairo | avoidablePropagation | 261.4051 |
| @vue/reactivity | kairo | broadPropagation | 534.6526 |
| @vue/reactivity | kairo | deepPropagation | 152.1300 |
| @vue/reactivity | kairo | diamond | 281.7336 |
| @vue/reactivity | kairo | mux | 434.9632 |
| @vue/reactivity | kairo | repeatedObservers | 26.0455 |
| @vue/reactivity | kairo | triangle | 93.3615 |
| @vue/reactivity | kairo | unstable | 63.9053 |
| @vue/reactivity | mol | molBench | 525.3353 |
| @vue/reactivity | s | createDataSignals | 9.5507 |
| @vue/reactivity | s | createComputations0to1 | 8.1643 |
| @vue/reactivity | s | createComputations1to1 | 20.5636 |
| @vue/reactivity | s | createComputations2to1 | 14.5406 |
| @vue/reactivity | s | createComputations4to1 | 12.9402 |
| @vue/reactivity | s | createComputations1000to1 | 13.4152 |
| @vue/reactivity | s | createComputations1to2 | 17.5439 |
| @vue/reactivity | s | createComputations1to4 | 14.7182 |
| @vue/reactivity | s | createComputations1to8 | 13.9566 |
| @vue/reactivity | s | createComputations1to1000 | 14.4874 |
| @vue/reactivity | s | updateComputations1to1 | 25.5878 |
| @vue/reactivity | s | updateComputations2to1 | 18.6657 |
| @vue/reactivity | s | updateComputations4to1 | 13.0931 |
| @vue/reactivity | s | updateComputations1000to1 | 7.9032 |
| @vue/reactivity | s | updateComputations1to2 | 21.0341 |
| @vue/reactivity | s | updateComputations1to4 | 19.3030 |
| @vue/reactivity | s | updateComputations1to1000 | 18.4167 |
| @vue/reactivity | dynamic | 10x5 - 2 sources - read 20% (simple component) | 404.8426 |
| @vue/reactivity | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 265.6525 |
| @vue/reactivity | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 446.3182 |
| @vue/reactivity | dynamic | 1000x5 - 25 sources (wide dense) | 784.5813 |
| @vue/reactivity | dynamic | 5x500 - 3 sources (deep) | 261.2566 |
| @vue/reactivity | cellx | cellx10 | 0.1267 |
| @vue/reactivity | cellx | cellx20 | 0.1827 |
| @vue/reactivity | cellx | cellx30 | 0.1195 |
| @pravosleva/reactive-engine | kairo | avoidablePropagation | 288.0453 |
| @pravosleva/reactive-engine | kairo | broadPropagation | 402.5316 |
| @pravosleva/reactive-engine | kairo | deepPropagation | 141.2046 |
| @pravosleva/reactive-engine | kairo | diamond | 236.8880 |
| @pravosleva/reactive-engine | kairo | mux | 329.2125 |
| @pravosleva/reactive-engine | kairo | repeatedObservers | 31.2001 |
| @pravosleva/reactive-engine | kairo | triangle | 78.1989 |
| @pravosleva/reactive-engine | kairo | unstable | 63.0029 |
| @pravosleva/reactive-engine | mol | molBench | 527.3795 |
| @pravosleva/reactive-engine | s | createDataSignals | 12.2007 |
| @pravosleva/reactive-engine | s | createComputations0to1 | 33.2006 |
| @pravosleva/reactive-engine | s | createComputations1to1 | 54.9979 |
| @pravosleva/reactive-engine | s | createComputations2to1 | 37.5860 |
| @pravosleva/reactive-engine | s | createComputations4to1 | 28.0569 |
| @pravosleva/reactive-engine | s | createComputations1000to1 | 129.0106 |
| @pravosleva/reactive-engine | s | createComputations1to2 | 47.1511 |
| @pravosleva/reactive-engine | s | createComputations1to4 | 43.7097 |
| @pravosleva/reactive-engine | s | createComputations1to8 | 41.7617 |
| @pravosleva/reactive-engine | s | createComputations1to1000 | 41.3677 |
| @pravosleva/reactive-engine | s | updateComputations1to1 | 58.0795 |
| @pravosleva/reactive-engine | s | updateComputations2to1 | 30.8959 |
| @pravosleva/reactive-engine | s | updateComputations4to1 | 17.1274 |
| @pravosleva/reactive-engine | s | updateComputations1000to1 | 3.4134 |
| @pravosleva/reactive-engine | s | updateComputations1to2 | 36.2607 |
| @pravosleva/reactive-engine | s | updateComputations1to4 | 26.3634 |
| @pravosleva/reactive-engine | s | updateComputations1to1000 | 16.9223 |
| @pravosleva/reactive-engine | dynamic | 10x5 - 2 sources - read 20% (simple component) | 408.7020 |
| @pravosleva/reactive-engine | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 180.8571 |
| @pravosleva/reactive-engine | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 340.1638 |
| @pravosleva/reactive-engine | dynamic | 1000x5 - 25 sources (wide dense) | 502.5280 |
| @pravosleva/reactive-engine | dynamic | 5x500 - 3 sources (deep) | 186.7674 |
| @pravosleva/reactive-engine | cellx | cellx10 | 0.0755 |
| @pravosleva/reactive-engine | cellx | cellx20 | 0.1021 |
| @pravosleva/reactive-engine | cellx | cellx30 | 0.1641 |
