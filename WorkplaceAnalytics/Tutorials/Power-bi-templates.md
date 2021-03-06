---
# Metadata Sample
# required metadata

title: Power BI templates
description: Use a Power BI template to run a query, export its results, and visualize them in Power BI
author: paul9955
ms.author: v-midehm
ms.date: 02/21/2019
ms.topic: article
localization_priority: normal 
ms.prod: wpa
---

# Power BI templates in Workplace Analytics

Workplace Analytics provides Power BI templates that analysts can use to visualize aspects of workplace patterns and trends. A Power BI template performs two tasks: it pre-populates a custom Workplace Analytics query and it selects the proper Power BI charts to display the results of that query.

The Queries page of Workplace Analytics has a number of predefined query templates available. On this page, you can identify Power BI templates by the Power BI logo in the upper-right corner:

   ![Power BI logo in query card](../Images/WpA/tutorials/two-pbi-cards.png)

For example, you can use the following steps to identify areas of collaboration overload in your organization with the Collaboration Overload query.

**To access a Power BI template**

1. In Workplace Analytics, select **Analyze** > **Queries**.
2. Select **Collaboration Overload** to open this predefined query, which has all the required metrics to populate the Power BI template.
3. Review the displayed metrics, which are required to populate the Power BI template.

   > [!Note] 
   > If you try to delete a metric, you'll see a warning that this deletion might disable portions of the Power BI template and reduce query results. In turn, this can limit your eventual ability to visualize collaboration-overload patterns. Depending on the metric you delete, you might disable a single Power BI chart, several charts, or all of the possible charts. In the warning dialog box, select **cancel** to retain the metric or **delete** to delete it.

4. Select a rule from the Meeting exclusions list. Optionally, select options for Group by, Time period, and Included employees.
5. Select **Run**. The query might take several minutes to complete.
6. Open the Query &gt; Results page. The Results page displays a row for every run of a query, including the query that you just ran. If your query is still running, this row displays the status as "running":

   ![Query is still running](../Images/WpA/tutorials/query-running.png)

 If the query has finished running, its row displays the download (down-arrow) button:

   ![Query results are ready](../Images/WpA/tutorials/query-results-done.png)
 
7. Select download. This gives you a choice of what to download, a CSV file or a Power BI template: 

   ![Select PBI template](../Images/WpA/tutorials/pbi-templates-03.png)

8. Select **PBI template**. This displays a dialog box that informs you that the OData link for this query has been copied to the clipboard. You will use this OData link in Power BI.
9. Select **OK** to dismiss the dialog box. The Power BI template query results file is now downloaded. 
10. In your browser, select the downloaded Power BI template query results file to open it:

   ![Open downloaded Power BI template file](../Images/WpA/tutorials/pbi-templates-05.png)

11. If a dialog box prompts you to select a program, choose **Power BI**.
12. After the query results file opens in Power BI and you're prompted, paste the OData link, and then select **Load**:

   ![Paste OData link here](../Images/WpA/tutorials/pbi-templates-07.png)

13. If you are already logged in to Power BI with your Workplace Analytics organizational account, your data loads and Power BI uses visualization charts to show your data. You are done and can _skip the following steps_.

   If you are not logged in to Power BI, the left panel of the **OData feed** dialog box highlights the current sign-in account for Power BI. For example, the following shows "Anonymous" as the sign-in account:

   ![Anonymous account displayed](../Images/WpA/tutorials/anon-access-to-pbi.png)

   > [!Important]
   > You can view Workplace Analytics data (including query results) in Power BI only if you've been assigned the Analyst role in Workplace Analytics. Also, you must sign in with the correct account with the following steps.

14. In the **OData feed** dialog box, select **Organizational account**.
15. If prompted, select **Sign in**.
16. In the **Office 365** dialog box, select the organizational account that you use to log in to Workplace Analytics. The **OData feed** dialog box shows "you are currently signed in" to Power BI:

   ![You are signed in](../Images/WpA/tutorials/you-are-signed-in.png)

17. Select **Connect** to show the status of the data preparation, which might take several minutes. After the data loads, Power BI uses visualization charts to show your organization’s collaboration patterns:

   ![Results visualized in Power BI](../Images/WpA/tutorials/pbi-templates-08a.png)

### Related topic

[View, download, and export query results](../use/view-download-and-export-query-results.md)