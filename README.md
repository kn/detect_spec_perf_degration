Detect Spec Performance Degration
=================================

This script allows you to detect performance degration of specified specs.

It runs the specs for every interval of revision in the past and compare the performance. It takes the biggest performance degration and operate git bisect on those two revisions to identify the commit that introduced the degration.

Usage
=====

For all specs in spec directly:
```
./detect_spec_perf_degration
```

For specs in a specific directly:
```
./detect_spec_perf_degration --spec spec/models
```

For a single spec:
```
./detect_spec_perf_degration --spec spec/models/user_spec.rb
```

For more customization:
```
./detect_spec_perf_degration -h
```
