Airflow pipeline consists of the following DAGs:
<br>
<p>get_data >> extract_gz >> fetch_pageviews >> write_to_postgres</p>
<p>
  <ul>
    <li>get_data - fetches the data in gzip format from wikimedia about user visits.</li>
    <li>extract_gz - extracts the data locally.</li>
    <li>fetch_pageviews - data for  {"Google", "Amazon", "Apple", "Microsoft", "Facebook"} regarding page views are collected and saved in sql file.</li>
    <li>write_to_postgres - previously saved data in sql file are inserted to PosgreSQL database (insert query from the file is executed).</li>
    
  </ul>
  
</p>

