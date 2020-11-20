## TRTCCloud

### 基础方法

| API                                                          | 描述                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [sharedInstance](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/sharedInstance.html) | 创建 TRTCCloud 单例。 |
| [destroySharedInstance](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/destroySharedInstance.html) | 销毁 TRTCCloud单例。 |
| [registerListener](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/registerListener.html) | 设置事件监听
| [unRegisterListener](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/unRegisterListener.html) | 移除事件监听

### 房间相关接口函数

| API                                                          | 描述                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [enterRoom](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/enterRoom.html) | 进入房间，若房间不存在，系统将自动创建一个新房间。           |
| [exitRoom](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/exitRoom.html) | 离开房间。                                                   |
| [switchRole](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/switchRole.html) | 切换角色，仅适用于直播场景（TRTC_APP_SCENE_LIVE 和 TRTC_APP_SCENE_VOICE_CHATROOM）。 |
| [setDefaultStreamRecvMode](http://doc.qcloudtrtc.com/group__TRTCCloud__android.html#a0b8d004665d5003ce1d9a48a9ab551b3) | 设置音视频数据接收模式，需要在进房前设置才能生效。           |


### CDN 相关接口函数

| API                                                          | 描述                          |
| ------------------------------------------------------------ | ----------------------------- |
| [setMixTranscodingConfig](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setMixTranscodingConfig.html) | 设置云端的混流转码参数。      |


### 视频相关接口函数

| API                                                          | 描述                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [startLocalPreview](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/startLocalPreview.html) | 开启本地视频的预览画面。                                     |
| [stopLocalPreview](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/stopLocalPreview.html) | 停止本地视频采集及预览。                                     |
| [muteLocalVideo](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/muteLocalVideo.html) | 暂停/恢复推送本地的视频数据。                                |
| [startRemoteView](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/startRemoteView.html) | 开始显示远端视频画面。                                       |
| [stopRemoteView](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/stopRemoteView.html) | 停止显示远端视频画面，同时不再拉取该远端用户的视频数据流。   |
| [stopAllRemoteView](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/stopAllRemoteView.html) | 停止显示所有远端视频画面，同时不再拉取远端用户的视频数据流。 |
| [muteRemoteVideoStream](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/muteRemoteVideoStream.html) | 暂停/恢复接收指定的远端视频流。                              |
| [muteAllRemoteVideoStreams](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/muteAllRemoteVideoStreams.html) | 暂停/恢复接收所有远端视频流。                                |
| [setVideoEncoderParam](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setVideoEncoderParam.html) | 设置视频编码器相关参数。                                     |
| [setNetworkQosParam](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setNetworkQosParam.html) | 设置网络流控相关参数。                                       |
| [setLocalRenderParams](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setLocalRenderParams.html) | 设置本地图像的渲染模式。 |
| [setRemoteRenderParams](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setRemoteRenderParams.html) | 设置远端图像相关参数。 |
| [setVideoEncoderRotation](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setVideoEncoderRotation.html) | 设置视频编码输出的画面方向，即设置远端用户观看到的和服务器录制的画面方向。 |
| [setVideoEncoderMirror](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setVideoEncoderMirror.html) | 设置编码器输出的画面镜像模式。 |
| [setGSensorMode](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setGSensorMode.html) | 设置重力感应的适应模式。 |
| [enableEncSmallVideoStream](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/enableEncSmallVideoStream.html) | 开启大小画面双路编码模式。 |
| [setRemoteVideoStreamType](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setRemoteVideoStreamType.html) | 选定观看指定 uid 的大画面或小画面。                          |
| [snapshotVideo](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/snapshotVideo.html) | 视频画面截图。 |


### 音频相关接口函数

| API                                                          | 描述                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [startLocalAudio](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/startLocalAudio.html) | 开启本地音频的采集和上行。                                   |
| [stopLocalAudio](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/stopLocalAudio.html) | 关闭本地音频的采集和上行。                                   |
| [muteLocalAudio](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/muteLocalAudio.html) | 静音/取消静音本地的音频。                                    |
| [setAudioRoute](https://pub.dev/documentation/tencent_trtc_cloud/latest/tx_device_manager/TXDeviceManager/setAudioRoute.html) | 设置音频路由。                                               |
| [muteRemoteAudio](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/muteRemoteAudio.html) | 静音/取消静音指定的远端用户的声音。                          |
| [muteAllRemoteAudio](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/muteAllRemoteAudio.html) | 静音/取消静音所有用户的声音。                                |
| [setAudioCaptureVolume](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setAudioCaptureVolume.html) | 设置 SDK 采集音量。                                          |
| [getAudioCaptureVolume](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/getAudioCaptureVolume.html) | 获取 SDK 采集音量。                                          |
| [setAudioPlayoutVolume](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setAudioPlayoutVolume.html) | 设置 SDK 播放音量。                                          |
| [getAudioPlayoutVolume](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/getAudioPlayoutVolume.html) | 获取 SDK 播放音量。                                          |
| [enableAudioVolumeEvaluation](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/enableAudioVolumeEvaluation.html) | 启用音量大小提示。                                           |
| [startAudioRecording](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/startAudioRecording.html) | 开始录音。                                                   |
| [stopAudioRecording](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/stopAudioRecording.html) | 停止录音。                                                   |
| [setSystemVolumeType](https://pub.dev/documentation/tencent_trtc_cloud/latest/tx_device_manager/TXDeviceManager/setSystemVolumeType.html) | 设置通话时使用的系统音量类型。                               |


### 设备管理接口

| API | 描述 |
|-----|-----|
| [getDeviceManager](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/getDeviceManager.html) | 获取设备管理模块。接口详情见[设备管理接口文档](https://pub.dev/documentation/tencent_trtc_cloud/latest/tx_device_manager/TXDeviceManager-class.html) |


### 美颜滤镜相关接口函数

| API                                                          | 描述               |
| ------------------------------------------------------------ | ------------------ |
| [getBeautyManager](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/getBeautyManager.html) | 获取美颜管理对象。接口详情见[美颜管理文档](https://pub.dev/documentation/tencent_trtc_cloud/latest/tx_beauty_manager/TXBeautyManager-class.html) |
| [setWatermark](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setWatermark.html) | 添加水印。         |


### 音乐特效和人声特效

| API                                                          | 描述                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [getAudioEffectManager](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/getAudioEffectManager.html) | 获取音效管理类 TXAudioEffectManager，用于管理BGM，短音效和人声特效。接口详情见[音效管理文档](https://pub.dev/documentation/tencent_trtc_cloud/latest/tx_audio_effect_manager/TXAudioEffectManager-class.html) |

### 网络测试

| API                                                          | 描述                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [startSpeedTest](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/startSpeedTest.html) | 开始进行网络测速（视频通话期间请勿测试，以免影响通话质量）。 |
| [stopSpeedTest](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/stopSpeedTest.html) | 停止服务器测速。                                             |


### Log 相关接口函数

| API                                                          | 描述                        |
| ------------------------------------------------------------ | --------------------------- |
| [getSDKVersion](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/getSDKVersion.html) | 获取 SDK 版本信息。         |
| [setLogLevel](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setLogLevel.html) | 设置 Log 输出级别。         |
| [setConsoleEnabled](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud/TRTCCloud/setConsoleEnabled.html) | 启用或禁用控制台日志打印。  |


## TRTCCloudListenerEnum

腾讯云视频通话功能的事件回调接口。

### 错误事件和警告事件

| API                                                          | 描述                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [onError](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 错误回调，表示 SDK 不可恢复的错误，一定要监听并分情况给用户适当的界面提示。 |
| [onWarning](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 警告回调，用于告知您一些非严重性问题，例如出现卡顿或者可恢复的解码失败。 |


### 房间事件回调

| API                                                          | 描述                                |
| ------------------------------------------------------------ | ----------------------------------- |
| [onEnterRoom](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 已加入房间的回调。                  |
| [onExitRoom](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 离开房间的事件回调。                |
| [onSwitchRole](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 切换角色的事件回调。                |


### 成员事件回调

| API                                                          | 描述                                                   |
| ------------------------------------------------------------ | ------------------------------------------------------ |
| [onRemoteUserEnterRoom](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 有用户加入当前房间。                                   |
| [onRemoteUserLeaveRoom](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 有用户离开当前房间。                                   |
| [onUserVideoAvailable](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 远端用户是否存在可播放的主路画面（一般用于摄像头）。   |
| [onUserSubStreamAvailable](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 远端用户是否存在可播放的辅路画面（一般用于屏幕分享）。 |
| [onUserAudioAvailable](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 远端用户是否存在可播放的音频数据。                     |
| [onFirstVideoFrame](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 开始渲染本地或远程用户的首帧画面。                     |
| [onFirstAudioFrame](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 开始播放远程用户的首帧音频（本地声音暂不通知）。       |
| [onSendFirstLocalVideoFrame](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 首帧本地视频数据已经被送出。                           |
| [onSendFirstLocalAudioFrame](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 首帧本地音频数据已经被送出。                           |

### 播放背景音乐的回调接口

播放背景音乐的回调接口。

| API                                                          | 描述                     |
| ------------------------------------------------------------ | ------------------------ |
| [onMusicObserverStart](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 音乐播放开始的回调通知。 |
| [onMusicObserverPlayProgress](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 音乐播放进度的回调通知。 |
| [onMusicObserverComplete](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 音乐播放结束的回调通知。 |

### 统计和质量回调

| API                                                          | 描述                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [onNetworkQuality](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 网络质量，该回调每2秒触发一次，统计当前网络的上行和下行质量。 |
| [onStatistics](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 技术指标统计回调。                                           |


### 服务器事件回调

| API                                                          | 描述                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [onConnectionLost](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | SDK 跟服务器的连接断开。                                     |
| [onTryToReconnect](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | SDK 尝试重新连接到服务器。                                   |
| [onConnectionRecovery](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | SDK 跟服务器的连接恢复。                                     |
| [onSpeedTest](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 服务器测速的回调，SDK 对多个服务器 IP 做测速，每个 IP 的测速结果通过这个回调通知。 |


### 硬件设备事件回调

| API                                                          | 描述                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [onCameraDidReady](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 摄像头准备就绪。                                             |
| [onMicDidReady](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 麦克风准备就绪。                                             |
| [onAudioRouteChanged](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 音频路由发生变化，音频路由即声音由哪里输出（扬声器或听筒）。 |
| [onUserVoiceVolume](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 用于提示音量大小的回调，包括每个 userId 的音量和远端总音量。 |


### CDN 旁路转推回调

| API                                                          | 描述                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [onSetMixTranscodingConfig](http://doc.qcloudtrtc.com/group__TRTCCloudListener__android.html#af1c79a5ec3e0c106939e7f0d7849d694) | 设置云端的混流转码参数的回调，对应于 [TRTCCloud](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) 中的 setMixTranscodingConfig() 接口。 |


### 截图回调

| API                                                          | 描述             |
| ------------------------------------------------------------ | ---------------- |
| [onSnapshotComplete](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_listener/TRTCCloudListenerEnum-class.html) | 截图完成时回调。 |


## 关键类型定义

| 类名                                                         | 描述                                    |
| ------------------------------------------------------------ | --------------------------------------- |
| [TRTCParams](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_def/TRTCParams-class.html) | 进房参数。                              |
| [TRTCVideoEncParam](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_def/TRTCVideoEncParam-class.html) | 编码参数。                              |
| [TRTCNetworkQosParam](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_def/TRTCNetworkQosParam-class.html) | 网络流控相关参数。                      |
| [TRTCRenderParams](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_def/TRTCRenderParams-class.html) | 远端图像参数。 |
| [TRTCMixUser](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_def/TRTCMixUser-class.html) | 云端混流中每一路子画面的位置信息。 |
| [TRTCTranscodingConfig](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_def/TRTCTranscodingConfig-class.html) | 云端混流（转码）配置。 |
| [TRTCAudioRecordingParams](https://pub.dev/documentation/tencent_trtc_cloud/latest/trtc_cloud_def/TRTCAudioRecordingParams-class.html) | 录音参数。 |