# Argo_Helm_Xgboost_EKS

Examples for results for EC2 bastion host

[ec2-user@ip-10-0-3-132 ~]$ curl http://a5e9a36b630d341c19294779f3efed14-1326651114.ap-southeast-2.elb.amazonaws.com/ping
{"status":"ok"}

[ec2-user@ip-10-0-3-132 ~]$ curl -H 'Content-Type: application/json' \
   -d '{"feature1": [1, 2, 3], "feature2": [4, 5, 6],"label": [7, 8, 9]}' \
   -X POST http://a5e9a36b630d341c19294779f3efed14-1326651114.ap-southeast-2.elb.amazonaws.com/invocations
[7.598736763000488,8.0,8.401262283325195]


[ec2-user@ip-10-0-3-132 ~]$ curl http://a5e9a36b630d341c19294779f3efed14-1326651114.ap-southeast-2.elb.amazonaws.com/metrics
python_gc_objects_collected_total{generation="0"} 825.0
python_gc_objects_collected_total{generation="1"} 236.0
python_gc_objects_collected_total{generation="2"} 0.0
python_gc_objects_uncollectable_total{generation="0"} 0.0
python_gc_objects_uncollectable_total{generation="1"} 0.0
python_gc_objects_uncollectable_total{generation="2"} 0.0
python_gc_collections_total{generation="0"} 222.0
python_gc_collections_total{generation="1"} 20.0
python_gc_collections_total{generation="2"} 1.0
python_info{implementation="CPython",major="3",minor="11",patchlevel="13",version="3.11.13"} 1.0
process_virtual_memory_bytes 7.22583552e+08
process_resident_memory_bytes 1.20979456e+08
process_start_time_seconds 1.75324555539e+09
process_cpu_seconds_total 0.98
process_open_fds 11.0
process_max_fds 65536.0
request_processing_seconds_count 0.0
request_processing_seconds_sum 0.0
request_processing_seconds_created 1.753245560248018e+09
cpu_usage_percent 1.7
memory_usage_percent 68.4
network_io_bytes_total{direction="in"} 1606.0
network_io_bytes_total{direction="out"} 1960.0
network_io_bytes_created{direction="in"} 1.7532462665754356e+09
network_io_bytes_created{direction="out"} 1.7532462665754535e+09

Argo UI for app deployments

<img width="1850" height="917" alt="image" src="https://github.com/user-attachments/assets/d373b8c8-3ccb-4657-b583-74c635d7a099" />

Flask app health check 
<img width="1044" height="182" alt="image" src="https://github.com/user-attachments/assets/9d1f7f6d-854e-45c0-8699-efaabc511921" />

Flask app metrics check 
<img width="1869" height="323" alt="image" src="https://github.com/user-attachments/assets/3e7dbba5-aa15-40a6-a429-98b280e30e98" />



