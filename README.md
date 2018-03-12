 data_expample = LOAD '$Server_name' USING PigStorage(',');
 filtered_data = FILTER data_example BY city = "Chicago";
 STORE filtered_data INTO '$des_server/dev/proc/cl/it USING HbaseStorage(',');
