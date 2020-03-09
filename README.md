# ProtoRandomWorkManager
WorkManagerを使いたかったときのプロトタイピングです。RoomとPagingのサンプルにもなるかも。  

This is project created to learning androidx.work.  
Androidx.workについて学ぶために作られたプロジェクトです。  

I wanted make sure below.  
確認したかったことは以下のことです。  

* WorkManager can register "Run periodically at random times of day" task.  
* WorkManagerは、「１日の内のランダムな時刻に定期的に実行される」タスクを登録できるか。  
* The Tasks are not overlapping by multitimes register.  
* そのタスクは、複数回登録しても重複することがないか。  

result, it can.  
結果は、可能でした。  
The task in this app, started 0 sec ~ 60 sec after app-launch, run every 15 min.  
このアプリのタスクは、アプリ起動後0秒から60秒で開始され、15分ごとに動作します。  

also using androidx.room to logging, androidx.paging to viewing.  
また、記録のためにandroidx.room、閲覧のためにandroidx.pagingを使っています。  

<img src="https://github.com/nredjap/ProtoRandomWorkManager/blob/master/document/ScreenShot.png" width=480px>
