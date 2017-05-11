
### json_each_text command
> - Examples:
> ```
> select d.key , d.value from gm2daq_odb join json_each_text(json_data->'Equipment'->'AMC1324'->'Common') 
> d on true  where run_num =5579;
> ```
> - Output:
> ```
>          key           |                                       value                                        
> -----------------------+------------------------------------------------------------------------------------
> Event ID/key           | { "type" : 4, "access_mode" : 7, "last_written" : 1493937548 }
> Event ID               | 0x0001
> Trigger mask/key       | { "type" : 4, "access_mode" : 7, "last_written" : 1493937548 }
> Trigger mask           | 0xffff
> Buffer/key             | { "type" : 12, "item_size" : 32, "access_mode" : 7, "last_written" : 1493937548 }
> Buffer                 | BUF24
> Type/key               | { "type" : 7, "access_mode" : 7, "last_written" : 1493937548 }
> Type                   | 130
> Source/key             | { "type" : 7, "access_mode" : 7, "last_written" : 1493937548 }
> Source                 | 16777215
> Format/key             | { "type" : 12, "item_size" : 8, "access_mode" : 7, "last_written" : 1493937548 }
> Format                 | MIDAS
> Enabled/key            | { "type" : 8, "notify_count" : 1, "access_mode" : 7, "last_written" : 1493937548 }
> Enabled                | true
> Read on/key            | { "type" : 7, "access_mode" : 7, "last_written" : 1493937548 }
> Read on                | 1
> Period/key             | { "type" : 7, "access_mode" : 7, "last_written" : 1493937548 }
> Period                 | 10
> Event limit/key        | { "type" : 10, "access_mode" : 7, "last_written" : 1493937548 }
> Event limit            | 0
> Num subevents/key      | { "type" : 6, "access_mode" : 7, "last_written" : 1493937548 }
> Num subevents          | 0x00000000
> Log history/key        | { "type" : 7, "access_mode" : 7, "last_written" : 1493937548 }
> Log history            | 0
> Frontend host/key      | { "type" : 12, "item_size" : 32, "access_mode" : 7, "last_written" : 1493937548 }
> Frontend host          | g2calo2324-data
> Frontend name/key      | { "type" : 12, "item_size" : 32, "access_mode" : 7, "last_written" : 1493937548 }
> Frontend name          | AMC1324
> Frontend file name/key | { "type" : 12, "item_size" : 256, "access_mode" : 7, "last_written" : 1493937548 }
> Frontend file name     | frontend.cpp
> Status/key             | { "type" : 12, "item_size" : 256, "access_mode" : 7, "last_written" : 1493937548 }
> Status                 | AMC1324@g2calo2324-data
> Status color/key       | { "type" : 12, "item_size" : 32, "access_mode" : 7, "last_written" : 1493939491 }
> Status color           | greenLight
> Hidden/key             | { "type" : 8, "access_mode" : 7, "last_written" : 1493937548 }
> Hidden                 | false
> ```
