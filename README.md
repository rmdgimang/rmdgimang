..projectviwsbot.//
using Google.Cloud.BigQuery.V2;
using System;

public class BigQueryQuery
{
    public void Query(
        string projectId = "your-project-id"
    )
    {
        BigQueryClient client = BigQueryClient.Create(projectId);
        string query = @"
            SELECT name FROM `bigquery-public-data.usa_names.usa_1910_2013`
            WHERE state = 'TX'
            LIMIT 100";
        BigQueryJob job = client.CreateQueryJob(
            sql: query,
            parameters: null,
            options: new QueryOptions { UseQueryCache = false });
        // Wait for the job to complete.
        job.PollUntilCompleted();
        // Display the results
        foreach (BigQueryRow row in client.GetQueryResults(job.Reference))
        {
            Console.WriteLine($"{row["name"]}");
        }
    }
}
        >youtube link< 
        link = linkInput.text():
@@ -40,6 +40,13 @@ def runBot():
    linkInput./UCGToazTIgmw9GbF_tu8nUzA<>
    linkInput.move(100, 25)

    timeLabel = QtWidgets.QLabel(win)
    timeLabel.setText("WatchTime(seconds)")
    timeLabel.move(15, 45)
    timeInput = QtWidgets.QLineEdit(win)
    timeInput.setGeometry(40, 10, 40, 20)
    timeInput.move(140, 55)

    runBotBtn = QtWidgets.QPushButton(win)
    runBotBtn.setGeometry(60, 270, 180, 40)
    runBotBtn.move(65, 80)       
    runBotBtn.setText("RUN VIEWBOT")
    runBotBtn.clicked.connect(runBot)
    win.show()
    sys.exit(app.exec_())
window()def check_and_log(method, self,
