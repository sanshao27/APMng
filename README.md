# APMng
Xposed 应用唤醒，Alarm,Wakelocks限制。应用后台活动限制。
<pre>
系统应用自动白名单（白名单检测函数isWhitelist）
关闭屏幕时立刻进入Doze模式(函数FastDoze)
禁止Provider或Broadcast,receiver形式启动应用。（函数RecvHook)
禁止后台应用使用revciver（函数RecvHook)
应用切换到后台自动冻结(FreezeTask)
禁止jobscheduler（被某些sdk用来应用保活自启(NoJobs)
应用从recent tasks中划出后就强行停止(HookTask)
Alarm,Wakelocks严格白名单(Syshook)
</pre>
