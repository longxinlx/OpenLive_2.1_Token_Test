# OpenLive for Android token test
0. 根据OpenLive修改
1. 修改app/src/main/res/values/strings_config.xml
   根据客户提供的数据，填充对应字段token，uid，channelname，appid
2. build两个不同apk（两套token，uid，根据同一个channelname生成，请客户提供）
3. 运行apk，joinchannel，提示框随意输入如：abc123（实际频道名为channelname）
4. 连麦成功，可查argus记录
5. 加入房间失败，onError请求会有错误码返回，通过adblogcat 打印
