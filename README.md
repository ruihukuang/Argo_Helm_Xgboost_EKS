# Argo_Helm_Xgboost_EKS

Examples for results 

[ec2-user@ip-10-0-3-132 ~]$ curl http://a5e9a36b630d341c19294779f3efed14-1326651114.ap-southeast-2.elb.amazonaws.com/ping
{"status":"ok"}

[ec2-user@ip-10-0-3-132 ~]$ curl -H 'Content-Type: application/json' \
>       -d '{"feature1": [1, 2, 3], "feature2": [4, 5, 6],"label": [7, 8, 9]}' \
>       -X POST http://a5e9a36b630d341c19294779f3efed14-1326651114.ap-southeast-2.elb.amazonaws.com/invocations
[7.598736763000488,8.0,8.401262283325195]


[ec2-user@ip-10-0-3-132 ~]$ curl http://a5e9a36b630d341c19294779f3efed14-1326651114.ap-southeast-2.elb.amazonaws.com/metrics
# HELP python_gc_objects_collected_total Objects collected during gc
# TYPE python_gc_objects_collected_total counter
python_gc_objects_collected_total{generation="0"} 825.0
python_gc_objects_collected_total{generation="1"} 236.0
python_gc_objects_collected_total{generation="2"} 0.0
# HELP python_gc_objects_uncollectable_total Uncollectable objects found during GC
# TYPE python_gc_objects_uncollectable_total counter
python_gc_objects_uncollectable_total{generation="0"} 0.0
python_gc_objects_uncollectable_total{generation="1"} 0.0
python_gc_objects_uncollectable_total{generation="2"} 0.0
# HELP python_gc_collections_total Number of times this generation was collected
# TYPE python_gc_collections_total counter
python_gc_collections_total{generation="0"} 222.0
python_gc_collections_total{generation="1"} 20.0
python_gc_collections_total{generation="2"} 1.0
# HELP python_info Python platform information
# TYPE python_info gauge
python_info{implementation="CPython",major="3",minor="11",patchlevel="13",version="3.11.13"} 1.0
# HELP process_virtual_memory_bytes Virtual memory size in bytes.
# TYPE process_virtual_memory_bytes gauge
process_virtual_memory_bytes 7.22583552e+08
# HELP process_resident_memory_bytes Resident memory size in bytes.
# TYPE process_resident_memory_bytes gauge
process_resident_memory_bytes 1.20979456e+08
# HELP process_start_time_seconds Start time of the process since unix epoch in seconds.
# TYPE process_start_time_seconds gauge
process_start_time_seconds 1.75324555539e+09
# HELP process_cpu_seconds_total Total user and system CPU time spent in seconds.
# TYPE process_cpu_seconds_total counter
process_cpu_seconds_total 0.98
# HELP process_open_fds Number of open file descriptors.
# TYPE process_open_fds gauge
process_open_fds 11.0
# HELP process_max_fds Maximum number of open file descriptors.
# TYPE process_max_fds gauge
process_max_fds 65536.0
# HELP request_processing_seconds Time spent processing request
# TYPE request_processing_seconds summary
request_processing_seconds_count 0.0
request_processing_seconds_sum 0.0
# HELP request_processing_seconds_created Time spent processing request
# TYPE request_processing_seconds_created gauge
request_processing_seconds_created 1.753245560248018e+09
# HELP cpu_usage_percent CPU usage percentage
# TYPE cpu_usage_percent gauge
cpu_usage_percent 1.7
# HELP memory_usage_percent Memory usage percentage
# TYPE memory_usage_percent gauge
memory_usage_percent 68.4
# HELP network_io_bytes_total Network I/O in bytes
# TYPE network_io_bytes_total counter
network_io_bytes_total{direction="in"} 1606.0
network_io_bytes_total{direction="out"} 1960.0
# HELP network_io_bytes_created Network I/O in bytes
# TYPE network_io_bytes_created gauge
network_io_bytes_created{direction="in"} 1.7532462665754356e+09
network_io_bytes_created{direction="out"} 1.7532462665754535e+09
