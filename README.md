
### json_each_text command
Examples:
select d.key , d.value from gm2daq_odb join json_each_text(json_data->'Equipment'->'AMC1324'->'Common') 
d on true  where run_num =5579;
