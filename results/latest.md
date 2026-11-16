# Benchmark snapshot

2026-11-16T19:01:45.959Z → 2026-11-16T19:16:36.664Z

**passed** · full · observed graphs · CellX standard

v24.22.2 · AMD EPYC 7763 64-Core Processor · linux x64

578 measurements; 0 failed suites. Times are milliseconds. Each framework/suite runs in a fresh process; values are the minimum of 3 samples. Explicit GC is outside timing. Raw samples are in the adjacent JSON file. See the repository README for workload definitions and limitations.

## Comparison by workload family

Geometric mean of each case's time divided by the fastest engine on that case. Lower is better; 1× means fastest on every case in that family. Cases have equal weight within a family. There is no overall score. Small CellX timings are particularly sensitive to noise.

| Engine | kairo | mol | s | dynamic | cellx |
| --- | ---: | ---: | ---: | ---: | ---: |
| alien-signals | 1.12× | 1.23× | 1.30× | 1.34× | 1.09× |
| @angular/signals | 3.50× | 1.27× | 3.39× | 3.97× | 1.98× |
| MobX | 4.81× | 1.28× | 4.43× | 3.95× | 3.66× |
| $mol_wire | 4.65× | 1.00× | 5.22× | 3.35× | 2.55× |
| Oby | 2.46× | 1.48× | 4.61× | 2.72× | 2.29× |
| Pota | 3.47× | 1.49× | 4.03× | 3.28× | 2.07× |
| reflex-quant | 1.00× | 1.20× | 1.00× | 1.00× | 1.00× |
| x-reactivity | 5.53× | 1.54× | 4.50× | 5.13× | 4.08× |
| Preact Signals | 1.32× | 1.22× | 1.59× | 1.86× | 1.73× |
| TC39 Signals Polyfill | 7.15× | 1.34× | 4.64× | 13.80× | 2.12× |
| SolidJS | 5.09× | 1.52× | 4.04× | 5.62× | 1.70× |
| Svelte v5 | 4.89× | 1.31× | 3.64× | 24.39× | 32.68× |
| @amadeus-it-group/tansu | 3.29× | 1.28× | 3.23× | 2.76× | 2.45× |
| @tldraw/state | 4.43× | 1.31× | 3.40× | 7.20× | 2.63× |
| uSignal | 3.55× | 1.72× | 3.02× | 3.26× | 2.11× |
| @vue/reactivity | 2.37× | 1.23× | 1.92× | 2.43× | 2.54× |
| @pravosleva/reactive-engine | 2.01× | 1.36× | 3.71× | 1.75× | 1.56× |

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
| alien-signals | kairo | avoidablePropagation | 134.5379 |
| alien-signals | kairo | broadPropagation | 274.2806 |
| alien-signals | kairo | deepPropagation | 91.2775 |
| alien-signals | kairo | diamond | 178.5417 |
| alien-signals | kairo | mux | 281.9422 |
| alien-signals | kairo | repeatedObservers | 21.9591 |
| alien-signals | kairo | triangle | 70.5956 |
| alien-signals | kairo | unstable | 71.5117 |
| alien-signals | mol | molBench | 648.1006 |
| alien-signals | s | createDataSignals | 7.8320 |
| alien-signals | s | createComputations0to1 | 6.0373 |
| alien-signals | s | createComputations1to1 | 14.9246 |
| alien-signals | s | createComputations2to1 | 12.3841 |
| alien-signals | s | createComputations4to1 | 12.7074 |
| alien-signals | s | createComputations1000to1 | 9.8600 |
| alien-signals | s | createComputations1to2 | 11.0495 |
| alien-signals | s | createComputations1to4 | 9.9668 |
| alien-signals | s | createComputations1to8 | 8.6315 |
| alien-signals | s | createComputations1to1000 | 13.9181 |
| alien-signals | s | updateComputations1to1 | 33.2630 |
| alien-signals | s | updateComputations2to1 | 19.8026 |
| alien-signals | s | updateComputations4to1 | 13.4175 |
| alien-signals | s | updateComputations1000to1 | 9.7067 |
| alien-signals | s | updateComputations1to2 | 24.6316 |
| alien-signals | s | updateComputations1to4 | 18.9123 |
| alien-signals | s | updateComputations1to1000 | 16.5464 |
| alien-signals | dynamic | 10x5 - 2 sources - read 20% (simple component) | 252.0860 |
| alien-signals | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 197.8619 |
| alien-signals | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 329.8603 |
| alien-signals | dynamic | 1000x5 - 25 sources (wide dense) | 624.2902 |
| alien-signals | dynamic | 5x500 - 3 sources (deep) | 170.0053 |
| alien-signals | cellx | cellx10 | 0.0858 |
| alien-signals | cellx | cellx20 | 0.0910 |
| alien-signals | cellx | cellx30 | 0.1090 |
| @angular/signals | kairo | avoidablePropagation | 485.5753 |
| @angular/signals | kairo | broadPropagation | 991.0559 |
| @angular/signals | kairo | deepPropagation | 276.5100 |
| @angular/signals | kairo | diamond | 615.2433 |
| @angular/signals | kairo | mux | 675.7608 |
| @angular/signals | kairo | repeatedObservers | 78.9395 |
| @angular/signals | kairo | triangle | 221.3340 |
| @angular/signals | kairo | unstable | 180.1897 |
| @angular/signals | mol | molBench | 669.3021 |
| @angular/signals | s | createDataSignals | 64.3390 |
| @angular/signals | s | createComputations0to1 | 12.5711 |
| @angular/signals | s | createComputations1to1 | 89.1151 |
| @angular/signals | s | createComputations2to1 | 80.9639 |
| @angular/signals | s | createComputations4to1 | 74.1926 |
| @angular/signals | s | createComputations1000to1 | 29.4375 |
| @angular/signals | s | createComputations1to2 | 36.4595 |
| @angular/signals | s | createComputations1to4 | 31.9202 |
| @angular/signals | s | createComputations1to8 | 29.3345 |
| @angular/signals | s | createComputations1to1000 | 21.2783 |
| @angular/signals | s | updateComputations1to1 | 43.7109 |
| @angular/signals | s | updateComputations2to1 | 28.3855 |
| @angular/signals | s | updateComputations4to1 | 21.3590 |
| @angular/signals | s | updateComputations1000to1 | 7.7756 |
| @angular/signals | s | updateComputations1to2 | 41.3792 |
| @angular/signals | s | updateComputations1to4 | 40.6102 |
| @angular/signals | s | updateComputations1to1000 | 36.5571 |
| @angular/signals | dynamic | 10x5 - 2 sources - read 20% (simple component) | 967.5339 |
| @angular/signals | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 527.2554 |
| @angular/signals | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 1120.3704 |
| @angular/signals | dynamic | 1000x5 - 25 sources (wide dense) | 1549.4772 |
| @angular/signals | dynamic | 5x500 - 3 sources (deep) | 444.4802 |
| @angular/signals | cellx | cellx10 | 0.1647 |
| @angular/signals | cellx | cellx20 | 0.1626 |
| @angular/signals | cellx | cellx30 | 0.1933 |
| MobX | kairo | avoidablePropagation | 707.4360 |
| MobX | kairo | broadPropagation | 1744.9910 |
| MobX | kairo | deepPropagation | 576.0347 |
| MobX | kairo | diamond | 909.9960 |
| MobX | kairo | mux | 750.5538 |
| MobX | kairo | repeatedObservers | 74.1473 |
| MobX | kairo | triangle | 296.5279 |
| MobX | kairo | unstable | 209.3295 |
| MobX | mol | molBench | 679.1816 |
| MobX | s | createDataSignals | 11.6821 |
| MobX | s | createComputations0to1 | 31.2641 |
| MobX | s | createComputations1to1 | 90.5267 |
| MobX | s | createComputations2to1 | 76.5852 |
| MobX | s | createComputations4to1 | 42.0380 |
| MobX | s | createComputations1000to1 | 18.9177 |
| MobX | s | createComputations1to2 | 87.3455 |
| MobX | s | createComputations1to4 | 69.5159 |
| MobX | s | createComputations1to8 | 62.9236 |
| MobX | s | createComputations1to1000 | 61.1303 |
| MobX | s | updateComputations1to1 | 85.2167 |
| MobX | s | updateComputations2to1 | 51.1795 |
| MobX | s | updateComputations4to1 | 29.9094 |
| MobX | s | updateComputations1000to1 | 7.4768 |
| MobX | s | updateComputations1to2 | 69.4753 |
| MobX | s | updateComputations1to4 | 62.2789 |
| MobX | s | updateComputations1to1000 | 56.0631 |
| MobX | dynamic | 10x5 - 2 sources - read 20% (simple component) | 1092.0641 |
| MobX | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 601.0017 |
| MobX | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 913.9613 |
| MobX | dynamic | 1000x5 - 25 sources (wide dense) | 1152.2332 |
| MobX | dynamic | 5x500 - 3 sources (deep) | 560.7362 |
| MobX | cellx | cellx10 | 0.1965 |
| MobX | cellx | cellx20 | 0.3531 |
| MobX | cellx | cellx30 | 0.4683 |
| $mol_wire | kairo | avoidablePropagation | 492.3693 |
| $mol_wire | kairo | broadPropagation | 1417.1165 |
| $mol_wire | kairo | deepPropagation | 399.2566 |
| $mol_wire | kairo | diamond | 689.1290 |
| $mol_wire | kairo | mux | 884.5424 |
| $mol_wire | kairo | repeatedObservers | 124.8365 |
| $mol_wire | kairo | triangle | 233.0200 |
| $mol_wire | kairo | unstable | 345.1243 |
| $mol_wire | mol | molBench | 529.0126 |
| $mol_wire | s | createDataSignals | 31.1621 |
| $mol_wire | s | createComputations0to1 | 21.3045 |
| $mol_wire | s | createComputations1to1 | 139.8469 |
| $mol_wire | s | createComputations2to1 | 56.3331 |
| $mol_wire | s | createComputations4to1 | 49.5904 |
| $mol_wire | s | createComputations1000to1 | 45.3901 |
| $mol_wire | s | createComputations1to2 | 81.5551 |
| $mol_wire | s | createComputations1to4 | 47.9574 |
| $mol_wire | s | createComputations1to8 | 40.4361 |
| $mol_wire | s | createComputations1to1000 | 35.7025 |
| $mol_wire | s | updateComputations1to1 | 121.5643 |
| $mol_wire | s | updateComputations2to1 | 70.4910 |
| $mol_wire | s | updateComputations4to1 | 42.2628 |
| $mol_wire | s | updateComputations1000to1 | 12.0445 |
| $mol_wire | s | updateComputations1to2 | 96.6728 |
| $mol_wire | s | updateComputations1to4 | 80.1182 |
| $mol_wire | s | updateComputations1to1000 | 79.0998 |
| $mol_wire | dynamic | 10x5 - 2 sources - read 20% (simple component) | 839.7467 |
| $mol_wire | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 430.7626 |
| $mol_wire | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 875.1623 |
| $mol_wire | dynamic | 1000x5 - 25 sources (wide dense) | 1124.3489 |
| $mol_wire | dynamic | 5x500 - 3 sources (deep) | 476.5160 |
| $mol_wire | cellx | cellx10 | 0.2366 |
| $mol_wire | cellx | cellx20 | 0.2027 |
| $mol_wire | cellx | cellx30 | 0.2303 |
| Oby | kairo | avoidablePropagation | 324.9142 |
| Oby | kairo | broadPropagation | 727.6248 |
| Oby | kairo | deepPropagation | 293.8560 |
| Oby | kairo | diamond | 418.7721 |
| Oby | kairo | mux | 423.3008 |
| Oby | kairo | repeatedObservers | 56.1326 |
| Oby | kairo | triangle | 159.0845 |
| Oby | kairo | unstable | 95.7123 |
| Oby | mol | molBench | 784.8777 |
| Oby | s | createDataSignals | 17.9053 |
| Oby | s | createComputations0to1 | 44.8125 |
| Oby | s | createComputations1to1 | 110.9570 |
| Oby | s | createComputations2to1 | 83.9449 |
| Oby | s | createComputations4to1 | 58.8393 |
| Oby | s | createComputations1000to1 | 20.0309 |
| Oby | s | createComputations1to2 | 83.7563 |
| Oby | s | createComputations1to4 | 80.7714 |
| Oby | s | createComputations1to8 | 82.2931 |
| Oby | s | createComputations1to1000 | 76.5270 |
| Oby | s | updateComputations1to1 | 56.2025 |
| Oby | s | updateComputations2to1 | 34.1531 |
| Oby | s | updateComputations4to1 | 21.6152 |
| Oby | s | updateComputations1000to1 | 16.8925 |
| Oby | s | updateComputations1to2 | 44.5889 |
| Oby | s | updateComputations1to4 | 41.5824 |
| Oby | s | updateComputations1to1000 | 43.7671 |
| Oby | dynamic | 10x5 - 2 sources - read 20% (simple component) | 621.0265 |
| Oby | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 414.6215 |
| Oby | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 736.6449 |
| Oby | dynamic | 1000x5 - 25 sources (wide dense) | 960.9591 |
| Oby | dynamic | 5x500 - 3 sources (deep) | 324.5988 |
| Oby | cellx | cellx10 | 0.1813 |
| Oby | cellx | cellx20 | 0.2777 |
| Oby | cellx | cellx30 | 0.1580 |
| Pota | kairo | avoidablePropagation | 628.8514 |
| Pota | kairo | broadPropagation | 797.6422 |
| Pota | kairo | deepPropagation | 302.3490 |
| Pota | kairo | diamond | 569.9930 |
| Pota | kairo | mux | 492.5124 |
| Pota | kairo | repeatedObservers | 118.4634 |
| Pota | kairo | triangle | 186.6998 |
| Pota | kairo | unstable | 173.9781 |
| Pota | mol | molBench | 788.6336 |
| Pota | s | createDataSignals | 14.7784 |
| Pota | s | createComputations0to1 | 15.2552 |
| Pota | s | createComputations1to1 | 78.4203 |
| Pota | s | createComputations2to1 | 75.1022 |
| Pota | s | createComputations4to1 | 75.8698 |
| Pota | s | createComputations1000to1 | 16.1666 |
| Pota | s | createComputations1to2 | 83.4971 |
| Pota | s | createComputations1to4 | 24.0139 |
| Pota | s | createComputations1to8 | 24.6939 |
| Pota | s | createComputations1to1000 | 21.0056 |
| Pota | s | updateComputations1to1 | 122.9629 |
| Pota | s | updateComputations2to1 | 74.5854 |
| Pota | s | updateComputations4to1 | 41.9734 |
| Pota | s | updateComputations1000to1 | 14.2032 |
| Pota | s | updateComputations1to2 | 85.0489 |
| Pota | s | updateComputations1to4 | 64.7794 |
| Pota | s | updateComputations1to1000 | 42.9545 |
| Pota | dynamic | 10x5 - 2 sources - read 20% (simple component) | 1028.6379 |
| Pota | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 508.7108 |
| Pota | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 669.0741 |
| Pota | dynamic | 1000x5 - 25 sources (wide dense) | 1048.7982 |
| Pota | dynamic | 5x500 - 3 sources (deep) | 417.4772 |
| Pota | cellx | cellx10 | 0.1308 |
| Pota | cellx | cellx20 | 0.2539 |
| Pota | cellx | cellx30 | 0.1784 |
| reflex-quant | kairo | avoidablePropagation | 118.3903 |
| reflex-quant | kairo | broadPropagation | 239.3931 |
| reflex-quant | kairo | deepPropagation | 93.4230 |
| reflex-quant | kairo | diamond | 166.7994 |
| reflex-quant | kairo | mux | 272.6330 |
| reflex-quant | kairo | repeatedObservers | 20.3442 |
| reflex-quant | kairo | triangle | 57.8020 |
| reflex-quant | kairo | unstable | 56.1955 |
| reflex-quant | mol | molBench | 637.2296 |
| reflex-quant | s | createDataSignals | 7.4532 |
| reflex-quant | s | createComputations0to1 | 5.7231 |
| reflex-quant | s | createComputations1to1 | 15.0318 |
| reflex-quant | s | createComputations2to1 | 12.0230 |
| reflex-quant | s | createComputations4to1 | 10.8540 |
| reflex-quant | s | createComputations1000to1 | 9.3440 |
| reflex-quant | s | createComputations1to2 | 10.7586 |
| reflex-quant | s | createComputations1to4 | 9.2528 |
| reflex-quant | s | createComputations1to8 | 8.0137 |
| reflex-quant | s | createComputations1to1000 | 8.2266 |
| reflex-quant | s | updateComputations1to1 | 22.7103 |
| reflex-quant | s | updateComputations2to1 | 13.6581 |
| reflex-quant | s | updateComputations4to1 | 9.0297 |
| reflex-quant | s | updateComputations1000to1 | 2.8023 |
| reflex-quant | s | updateComputations1to2 | 15.7516 |
| reflex-quant | s | updateComputations1to4 | 14.2377 |
| reflex-quant | s | updateComputations1to1000 | 13.5144 |
| reflex-quant | dynamic | 10x5 - 2 sources - read 20% (simple component) | 210.0392 |
| reflex-quant | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 157.7719 |
| reflex-quant | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 235.8891 |
| reflex-quant | dynamic | 1000x5 - 25 sources (wide dense) | 357.7914 |
| reflex-quant | dynamic | 5x500 - 3 sources (deep) | 143.3220 |
| reflex-quant | cellx | cellx10 | 0.0834 |
| reflex-quant | cellx | cellx20 | 0.0887 |
| reflex-quant | cellx | cellx30 | 0.0898 |
| x-reactivity | kairo | avoidablePropagation | 757.3605 |
| x-reactivity | kairo | broadPropagation | 1597.0681 |
| x-reactivity | kairo | deepPropagation | 537.4458 |
| x-reactivity | kairo | diamond | 1070.6690 |
| x-reactivity | kairo | mux | 547.2367 |
| x-reactivity | kairo | repeatedObservers | 172.2105 |
| x-reactivity | kairo | triangle | 366.6206 |
| x-reactivity | kairo | unstable | 282.9119 |
| x-reactivity | mol | molBench | 812.3132 |
| x-reactivity | s | createDataSignals | 14.8163 |
| x-reactivity | s | createComputations0to1 | 15.8106 |
| x-reactivity | s | createComputations1to1 | 85.4432 |
| x-reactivity | s | createComputations2to1 | 69.4275 |
| x-reactivity | s | createComputations4to1 | 23.0937 |
| x-reactivity | s | createComputations1000to1 | 18.5082 |
| x-reactivity | s | createComputations1to2 | 36.4613 |
| x-reactivity | s | createComputations1to4 | 25.3648 |
| x-reactivity | s | createComputations1to8 | 24.5357 |
| x-reactivity | s | createComputations1to1000 | 21.7498 |
| x-reactivity | s | updateComputations1to1 | 228.0076 |
| x-reactivity | s | updateComputations2to1 | 127.2327 |
| x-reactivity | s | updateComputations4to1 | 67.8838 |
| x-reactivity | s | updateComputations1000to1 | 17.1003 |
| x-reactivity | s | updateComputations1to2 | 160.3797 |
| x-reactivity | s | updateComputations1to4 | 116.2674 |
| x-reactivity | s | updateComputations1to1000 | 78.7178 |
| x-reactivity | dynamic | 10x5 - 2 sources - read 20% (simple component) | 2772.1023 |
| x-reactivity | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 686.0132 |
| x-reactivity | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 1088.4053 |
| x-reactivity | dynamic | 1000x5 - 25 sources (wide dense) | 1392.2848 |
| x-reactivity | dynamic | 5x500 - 3 sources (deep) | 493.6133 |
| x-reactivity | cellx | cellx10 | 0.2844 |
| x-reactivity | cellx | cellx20 | 0.6333 |
| x-reactivity | cellx | cellx30 | 0.2500 |
| Preact Signals | kairo | avoidablePropagation | 179.5904 |
| Preact Signals | kairo | broadPropagation | 317.3637 |
| Preact Signals | kairo | deepPropagation | 118.5290 |
| Preact Signals | kairo | diamond | 264.0588 |
| Preact Signals | kairo | mux | 311.1101 |
| Preact Signals | kairo | repeatedObservers | 23.6723 |
| Preact Signals | kairo | triangle | 89.7571 |
| Preact Signals | kairo | unstable | 60.2948 |
| Preact Signals | mol | molBench | 645.8919 |
| Preact Signals | s | createDataSignals | 9.6451 |
| Preact Signals | s | createComputations0to1 | 10.0685 |
| Preact Signals | s | createComputations1to1 | 29.8259 |
| Preact Signals | s | createComputations2to1 | 19.0194 |
| Preact Signals | s | createComputations4to1 | 12.7986 |
| Preact Signals | s | createComputations1000to1 | 13.1951 |
| Preact Signals | s | createComputations1to2 | 18.4217 |
| Preact Signals | s | createComputations1to4 | 17.4466 |
| Preact Signals | s | createComputations1to8 | 15.5152 |
| Preact Signals | s | createComputations1to1000 | 16.6779 |
| Preact Signals | s | updateComputations1to1 | 30.8282 |
| Preact Signals | s | updateComputations2to1 | 20.1627 |
| Preact Signals | s | updateComputations4to1 | 15.8148 |
| Preact Signals | s | updateComputations1000to1 | 6.9173 |
| Preact Signals | s | updateComputations1to2 | 21.0578 |
| Preact Signals | s | updateComputations1to4 | 18.0283 |
| Preact Signals | s | updateComputations1to1000 | 15.1093 |
| Preact Signals | dynamic | 10x5 - 2 sources - read 20% (simple component) | 401.9404 |
| Preact Signals | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 278.5864 |
| Preact Signals | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 471.9216 |
| Preact Signals | dynamic | 1000x5 - 25 sources (wide dense) | 722.7366 |
| Preact Signals | dynamic | 5x500 - 3 sources (deep) | 231.5250 |
| Preact Signals | cellx | cellx10 | 0.1398 |
| Preact Signals | cellx | cellx20 | 0.1308 |
| Preact Signals | cellx | cellx30 | 0.1872 |
| TC39 Signals Polyfill | kairo | avoidablePropagation | 707.9062 |
| TC39 Signals Polyfill | kairo | broadPropagation | 1735.5079 |
| TC39 Signals Polyfill | kairo | deepPropagation | 454.6336 |
| TC39 Signals Polyfill | kairo | diamond | 935.4470 |
| TC39 Signals Polyfill | kairo | mux | 1108.9447 |
| TC39 Signals Polyfill | kairo | repeatedObservers | 265.6850 |
| TC39 Signals Polyfill | kairo | triangle | 340.4417 |
| TC39 Signals Polyfill | kairo | unstable | 1013.9361 |
| TC39 Signals Polyfill | mol | molBench | 710.4074 |
| TC39 Signals Polyfill | s | createDataSignals | 25.1637 |
| TC39 Signals Polyfill | s | createComputations0to1 | 39.5303 |
| TC39 Signals Polyfill | s | createComputations1to1 | 90.0795 |
| TC39 Signals Polyfill | s | createComputations2to1 | 52.8019 |
| TC39 Signals Polyfill | s | createComputations4to1 | 40.8016 |
| TC39 Signals Polyfill | s | createComputations1000to1 | 27.1926 |
| TC39 Signals Polyfill | s | createComputations1to2 | 69.4047 |
| TC39 Signals Polyfill | s | createComputations1to4 | 59.6789 |
| TC39 Signals Polyfill | s | createComputations1to8 | 58.9062 |
| TC39 Signals Polyfill | s | createComputations1to1000 | 52.8958 |
| TC39 Signals Polyfill | s | updateComputations1to1 | 76.3908 |
| TC39 Signals Polyfill | s | updateComputations2to1 | 47.6918 |
| TC39 Signals Polyfill | s | updateComputations4to1 | 35.8974 |
| TC39 Signals Polyfill | s | updateComputations1000to1 | 12.8450 |
| TC39 Signals Polyfill | s | updateComputations1to2 | 75.5454 |
| TC39 Signals Polyfill | s | updateComputations1to4 | 56.7544 |
| TC39 Signals Polyfill | s | updateComputations1to1000 | 48.8207 |
| TC39 Signals Polyfill | dynamic | 10x5 - 2 sources - read 20% (simple component) | 2445.4169 |
| TC39 Signals Polyfill | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 794.9067 |
| TC39 Signals Polyfill | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 15607.9164 |
| TC39 Signals Polyfill | dynamic | 1000x5 - 25 sources (wide dense) | 10568.7194 |
| TC39 Signals Polyfill | dynamic | 5x500 - 3 sources (deep) | 626.5788 |
| TC39 Signals Polyfill | cellx | cellx10 | 0.1453 |
| TC39 Signals Polyfill | cellx | cellx20 | 0.3124 |
| TC39 Signals Polyfill | cellx | cellx30 | 0.1400 |
| SolidJS | kairo | avoidablePropagation | 729.8491 |
| SolidJS | kairo | broadPropagation | 1560.1864 |
| SolidJS | kairo | deepPropagation | 627.3828 |
| SolidJS | kairo | diamond | 979.7842 |
| SolidJS | kairo | mux | 739.0820 |
| SolidJS | kairo | repeatedObservers | 125.3229 |
| SolidJS | kairo | triangle | 290.9335 |
| SolidJS | kairo | unstable | 185.8957 |
| SolidJS | mol | molBench | 806.1247 |
| SolidJS | s | createDataSignals | 12.3991 |
| SolidJS | s | createComputations0to1 | 13.9461 |
| SolidJS | s | createComputations1to1 | 75.2488 |
| SolidJS | s | createComputations2to1 | 66.4609 |
| SolidJS | s | createComputations4to1 | 47.2659 |
| SolidJS | s | createComputations1000to1 | 11.6870 |
| SolidJS | s | createComputations1to2 | 68.1513 |
| SolidJS | s | createComputations1to4 | 21.6892 |
| SolidJS | s | createComputations1to8 | 18.0508 |
| SolidJS | s | createComputations1to1000 | 15.3108 |
| SolidJS | s | updateComputations1to1 | 141.6423 |
| SolidJS | s | updateComputations2to1 | 92.6206 |
| SolidJS | s | updateComputations4to1 | 65.5186 |
| SolidJS | s | updateComputations1000to1 | 40.5934 |
| SolidJS | s | updateComputations1to2 | 83.5907 |
| SolidJS | s | updateComputations1to4 | 70.2879 |
| SolidJS | s | updateComputations1to1000 | 58.4354 |
| SolidJS | dynamic | 10x5 - 2 sources - read 20% (simple component) | 2666.8849 |
| SolidJS | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 853.8811 |
| SolidJS | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 970.5198 |
| SolidJS | dynamic | 1000x5 - 25 sources (wide dense) | 1707.8374 |
| SolidJS | dynamic | 5x500 - 3 sources (deep) | 596.2291 |
| SolidJS | cellx | cellx10 | 0.1659 |
| SolidJS | cellx | cellx20 | 0.1794 |
| SolidJS | cellx | cellx30 | 0.1090 |
| Svelte v5 | kairo | avoidablePropagation | 1029.9084 |
| Svelte v5 | kairo | broadPropagation | 1253.3815 |
| Svelte v5 | kairo | deepPropagation | 504.1409 |
| Svelte v5 | kairo | diamond | 1036.7905 |
| Svelte v5 | kairo | mux | 417.9893 |
| Svelte v5 | kairo | repeatedObservers | 127.5452 |
| Svelte v5 | kairo | triangle | 331.8655 |
| Svelte v5 | kairo | unstable | 211.6223 |
| Svelte v5 | mol | molBench | 694.0259 |
| Svelte v5 | s | createDataSignals | 8.4978 |
| Svelte v5 | s | createComputations0to1 | 36.0913 |
| Svelte v5 | s | createComputations1to1 | 45.8938 |
| Svelte v5 | s | createComputations2to1 | 28.8359 |
| Svelte v5 | s | createComputations4to1 | 18.2593 |
| Svelte v5 | s | createComputations1000to1 | 8.7030 |
| Svelte v5 | s | createComputations1to2 | 34.3047 |
| Svelte v5 | s | createComputations1to4 | 31.4242 |
| Svelte v5 | s | createComputations1to8 | 30.7720 |
| Svelte v5 | s | createComputations1to1000 | 26.6832 |
| Svelte v5 | s | updateComputations1to1 | 263.8417 |
| Svelte v5 | s | updateComputations2to1 | 135.1203 |
| Svelte v5 | s | updateComputations4to1 | 70.3012 |
| Svelte v5 | s | updateComputations1000to1 | 6.2610 |
| Svelte v5 | s | updateComputations1to2 | 148.2388 |
| Svelte v5 | s | updateComputations1to4 | 91.5803 |
| Svelte v5 | s | updateComputations1to1000 | 32.5170 |
| Svelte v5 | dynamic | 10x5 - 2 sources - read 20% (simple component) | 1250.1618 |
| Svelte v5 | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 26455.1739 |
| Svelte v5 | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 12605.5247 |
| Svelte v5 | dynamic | 1000x5 - 25 sources (wide dense) | 5901.7297 |
| Svelte v5 | dynamic | 5x500 - 3 sources (deep) | 1404.8019 |
| Svelte v5 | cellx | cellx10 | 0.3505 |
| Svelte v5 | cellx | cellx20 | 6.8683 |
| Svelte v5 | cellx | cellx30 | 9.6333 |
| @amadeus-it-group/tansu | kairo | avoidablePropagation | 449.4775 |
| @amadeus-it-group/tansu | kairo | broadPropagation | 932.9937 |
| @amadeus-it-group/tansu | kairo | deepPropagation | 293.4113 |
| @amadeus-it-group/tansu | kairo | diamond | 464.7654 |
| @amadeus-it-group/tansu | kairo | mux | 667.4349 |
| @amadeus-it-group/tansu | kairo | repeatedObservers | 83.4992 |
| @amadeus-it-group/tansu | kairo | triangle | 147.0503 |
| @amadeus-it-group/tansu | kairo | unstable | 225.3799 |
| @amadeus-it-group/tansu | mol | molBench | 677.8256 |
| @amadeus-it-group/tansu | s | createDataSignals | 17.1989 |
| @amadeus-it-group/tansu | s | createComputations0to1 | 18.8159 |
| @amadeus-it-group/tansu | s | createComputations1to1 | 77.7740 |
| @amadeus-it-group/tansu | s | createComputations2to1 | 47.4480 |
| @amadeus-it-group/tansu | s | createComputations4to1 | 24.7320 |
| @amadeus-it-group/tansu | s | createComputations1000to1 | 26.7038 |
| @amadeus-it-group/tansu | s | createComputations1to2 | 52.0463 |
| @amadeus-it-group/tansu | s | createComputations1to4 | 42.6722 |
| @amadeus-it-group/tansu | s | createComputations1to8 | 38.0337 |
| @amadeus-it-group/tansu | s | createComputations1to1000 | 32.2016 |
| @amadeus-it-group/tansu | s | updateComputations1to1 | 50.7127 |
| @amadeus-it-group/tansu | s | updateComputations2to1 | 31.8533 |
| @amadeus-it-group/tansu | s | updateComputations4to1 | 20.1763 |
| @amadeus-it-group/tansu | s | updateComputations1000to1 | 9.6970 |
| @amadeus-it-group/tansu | s | updateComputations1to2 | 44.1404 |
| @amadeus-it-group/tansu | s | updateComputations1to4 | 41.7710 |
| @amadeus-it-group/tansu | s | updateComputations1to1000 | 41.4174 |
| @amadeus-it-group/tansu | dynamic | 10x5 - 2 sources - read 20% (simple component) | 707.3159 |
| @amadeus-it-group/tansu | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 354.3383 |
| @amadeus-it-group/tansu | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 785.0654 |
| @amadeus-it-group/tansu | dynamic | 1000x5 - 25 sources (wide dense) | 930.8070 |
| @amadeus-it-group/tansu | dynamic | 5x500 - 3 sources (deep) | 348.5678 |
| @amadeus-it-group/tansu | cellx | cellx10 | 0.2070 |
| @amadeus-it-group/tansu | cellx | cellx20 | 0.1860 |
| @amadeus-it-group/tansu | cellx | cellx30 | 0.2536 |
| @tldraw/state | kairo | avoidablePropagation | 598.8291 |
| @tldraw/state | kairo | broadPropagation | 1269.6373 |
| @tldraw/state | kairo | deepPropagation | 418.8276 |
| @tldraw/state | kairo | diamond | 793.7081 |
| @tldraw/state | kairo | mux | 784.8972 |
| @tldraw/state | kairo | repeatedObservers | 99.1131 |
| @tldraw/state | kairo | triangle | 340.5458 |
| @tldraw/state | kairo | unstable | 171.5332 |
| @tldraw/state | mol | molBench | 690.3808 |
| @tldraw/state | s | createDataSignals | 13.4141 |
| @tldraw/state | s | createComputations0to1 | 11.6158 |
| @tldraw/state | s | createComputations1to1 | 30.6803 |
| @tldraw/state | s | createComputations2to1 | 28.2926 |
| @tldraw/state | s | createComputations4to1 | 13.6444 |
| @tldraw/state | s | createComputations1000to1 | 23.0675 |
| @tldraw/state | s | createComputations1to2 | 27.7014 |
| @tldraw/state | s | createComputations1to4 | 25.9813 |
| @tldraw/state | s | createComputations1to8 | 26.9133 |
| @tldraw/state | s | createComputations1to1000 | 24.1151 |
| @tldraw/state | s | updateComputations1to1 | 123.6827 |
| @tldraw/state | s | updateComputations2to1 | 73.6728 |
| @tldraw/state | s | updateComputations4to1 | 50.1327 |
| @tldraw/state | s | updateComputations1000to1 | 28.3539 |
| @tldraw/state | s | updateComputations1to2 | 96.3440 |
| @tldraw/state | s | updateComputations1to4 | 79.4085 |
| @tldraw/state | s | updateComputations1to1000 | 61.8295 |
| @tldraw/state | dynamic | 10x5 - 2 sources - read 20% (simple component) | 1139.5407 |
| @tldraw/state | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 593.4732 |
| @tldraw/state | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 5266.8113 |
| @tldraw/state | dynamic | 1000x5 - 25 sources (wide dense) | 4748.3246 |
| @tldraw/state | dynamic | 5x500 - 3 sources (deep) | 459.7354 |
| @tldraw/state | cellx | cellx10 | 0.1688 |
| @tldraw/state | cellx | cellx20 | 0.3317 |
| @tldraw/state | cellx | cellx30 | 0.2161 |
| uSignal | kairo | avoidablePropagation | 822.2919 |
| uSignal | kairo | broadPropagation | 1041.5319 |
| uSignal | kairo | deepPropagation | 332.6646 |
| uSignal | kairo | diamond | 539.7089 |
| uSignal | kairo | mux | 842.4127 |
| uSignal | kairo | repeatedObservers | 73.2890 |
| uSignal | kairo | triangle | 208.9639 |
| uSignal | kairo | unstable | 99.2578 |
| uSignal | mol | molBench | 911.6657 |
| uSignal | s | createDataSignals | 13.2734 |
| uSignal | s | createComputations0to1 | 13.8830 |
| uSignal | s | createComputations1to1 | 65.3254 |
| uSignal | s | createComputations2to1 | 30.4014 |
| uSignal | s | createComputations4to1 | 20.8779 |
| uSignal | s | createComputations1000to1 | 19.1765 |
| uSignal | s | createComputations1to2 | 59.2550 |
| uSignal | s | createComputations1to4 | 37.6420 |
| uSignal | s | createComputations1to8 | 36.4627 |
| uSignal | s | createComputations1to1000 | 19.8711 |
| uSignal | s | updateComputations1to1 | 57.6642 |
| uSignal | s | updateComputations2to1 | 36.8959 |
| uSignal | s | updateComputations4to1 | 23.1115 |
| uSignal | s | updateComputations1000to1 | 14.5954 |
| uSignal | s | updateComputations1to2 | 47.1136 |
| uSignal | s | updateComputations1to4 | 43.0981 |
| uSignal | s | updateComputations1to1000 | 47.3280 |
| uSignal | dynamic | 10x5 - 2 sources - read 20% (simple component) | 648.4864 |
| uSignal | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 586.2965 |
| uSignal | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 681.3516 |
| uSignal | dynamic | 1000x5 - 25 sources (wide dense) | 1507.5628 |
| uSignal | dynamic | 5x500 - 3 sources (deep) | 377.8480 |
| uSignal | cellx | cellx10 | 0.1446 |
| uSignal | cellx | cellx20 | 0.2257 |
| uSignal | cellx | cellx30 | 0.1903 |
| @vue/reactivity | kairo | avoidablePropagation | 455.9296 |
| @vue/reactivity | kairo | broadPropagation | 733.4384 |
| @vue/reactivity | kairo | deepPropagation | 206.5656 |
| @vue/reactivity | kairo | diamond | 440.0949 |
| @vue/reactivity | kairo | mux | 538.5707 |
| @vue/reactivity | kairo | repeatedObservers | 40.5037 |
| @vue/reactivity | kairo | triangle | 128.9567 |
| @vue/reactivity | kairo | unstable | 91.1157 |
| @vue/reactivity | mol | molBench | 651.2389 |
| @vue/reactivity | s | createDataSignals | 12.6231 |
| @vue/reactivity | s | createComputations0to1 | 8.9238 |
| @vue/reactivity | s | createComputations1to1 | 27.1557 |
| @vue/reactivity | s | createComputations2to1 | 24.7567 |
| @vue/reactivity | s | createComputations4to1 | 15.5108 |
| @vue/reactivity | s | createComputations1000to1 | 17.4963 |
| @vue/reactivity | s | createComputations1to2 | 22.7195 |
| @vue/reactivity | s | createComputations1to4 | 20.4606 |
| @vue/reactivity | s | createComputations1to8 | 17.8053 |
| @vue/reactivity | s | createComputations1to1000 | 18.5387 |
| @vue/reactivity | s | updateComputations1to1 | 35.8863 |
| @vue/reactivity | s | updateComputations2to1 | 23.4791 |
| @vue/reactivity | s | updateComputations4to1 | 16.6794 |
| @vue/reactivity | s | updateComputations1000to1 | 10.3445 |
| @vue/reactivity | s | updateComputations1to2 | 26.5144 |
| @vue/reactivity | s | updateComputations1to4 | 25.2987 |
| @vue/reactivity | s | updateComputations1to1000 | 23.1927 |
| @vue/reactivity | dynamic | 10x5 - 2 sources - read 20% (simple component) | 563.8681 |
| @vue/reactivity | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 334.6798 |
| @vue/reactivity | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 602.8722 |
| @vue/reactivity | dynamic | 1000x5 - 25 sources (wide dense) | 930.8600 |
| @vue/reactivity | dynamic | 5x500 - 3 sources (deep) | 321.6927 |
| @vue/reactivity | cellx | cellx10 | 0.1780 |
| @vue/reactivity | cellx | cellx20 | 0.2479 |
| @vue/reactivity | cellx | cellx30 | 0.2455 |
| @pravosleva/reactive-engine | kairo | avoidablePropagation | 424.7194 |
| @pravosleva/reactive-engine | kairo | broadPropagation | 486.2578 |
| @pravosleva/reactive-engine | kairo | deepPropagation | 169.4256 |
| @pravosleva/reactive-engine | kairo | diamond | 337.9418 |
| @pravosleva/reactive-engine | kairo | mux | 423.2470 |
| @pravosleva/reactive-engine | kairo | repeatedObservers | 44.4495 |
| @pravosleva/reactive-engine | kairo | triangle | 107.0024 |
| @pravosleva/reactive-engine | kairo | unstable | 88.3385 |
| @pravosleva/reactive-engine | mol | molBench | 717.6407 |
| @pravosleva/reactive-engine | s | createDataSignals | 15.0035 |
| @pravosleva/reactive-engine | s | createComputations0to1 | 39.0102 |
| @pravosleva/reactive-engine | s | createComputations1to1 | 65.0997 |
| @pravosleva/reactive-engine | s | createComputations2to1 | 43.2539 |
| @pravosleva/reactive-engine | s | createComputations4to1 | 34.4494 |
| @pravosleva/reactive-engine | s | createComputations1000to1 | 154.0692 |
| @pravosleva/reactive-engine | s | createComputations1to2 | 56.9455 |
| @pravosleva/reactive-engine | s | createComputations1to4 | 52.5687 |
| @pravosleva/reactive-engine | s | createComputations1to8 | 51.3143 |
| @pravosleva/reactive-engine | s | createComputations1to1000 | 48.5457 |
| @pravosleva/reactive-engine | s | updateComputations1to1 | 74.1785 |
| @pravosleva/reactive-engine | s | updateComputations2to1 | 40.5226 |
| @pravosleva/reactive-engine | s | updateComputations4to1 | 22.2885 |
| @pravosleva/reactive-engine | s | updateComputations1000to1 | 4.1660 |
| @pravosleva/reactive-engine | s | updateComputations1to2 | 46.2186 |
| @pravosleva/reactive-engine | s | updateComputations1to4 | 32.2966 |
| @pravosleva/reactive-engine | s | updateComputations1to1000 | 20.1377 |
| @pravosleva/reactive-engine | dynamic | 10x5 - 2 sources - read 20% (simple component) | 503.9035 |
| @pravosleva/reactive-engine | dynamic | 10x10 - 6 sources - dynamic - read 20% (dynamic component) | 221.6556 |
| @pravosleva/reactive-engine | dynamic | 1000x12 - 4 sources - dynamic (large web app) | 424.5972 |
| @pravosleva/reactive-engine | dynamic | 1000x5 - 25 sources (wide dense) | 603.1839 |
| @pravosleva/reactive-engine | dynamic | 5x500 - 3 sources (deep) | 227.3596 |
| @pravosleva/reactive-engine | cellx | cellx10 | 0.1034 |
| @pravosleva/reactive-engine | cellx | cellx20 | 0.1415 |
| @pravosleva/reactive-engine | cellx | cellx30 | 0.1730 |
