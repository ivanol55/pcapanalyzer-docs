# queryRunner SQL form

In the `queryRunner` tab of the web fronend, you get a text field where you can write your own SQL `SELECT` query, in the event that the `packetstream` table is limited for your needs. You need to write your SQL query inside of the text field on the page (as specified, the data table is always named `main`), and when it's done, click on the `Run query` button to run it. Once done, your browser will prompt you to download a CSV file with your data.

The database that the query runs on is dependent on what is your current session's selected database to work with, indicated on the top menu bar, on the `Current database` menu button.

This input field will only run `SELECT` queries on the selected database. Any other query order type will return an error.
