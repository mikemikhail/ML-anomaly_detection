$ sudo influxd restore -portable -db mdt_db -newdb mdt_db-200116 -retention INF .
then change database retention to INF
After that you can go in Grafana to Configuration > Data Sources > InfluxDB > Database > change to mdt_db-200116 > Save & Test
so you can visualize in dashboards for the data between Dec 24, 2019 and Jan 16, 2020.

This is a backup of influxdb database mdt_db. With data for 24 days ending Jan 16th, 2020.
One measurement which is interface generic counters, from 6 XRv9K edge nodes. Including tunnel-te overlay.

To restore https://www.influxdata.com/blog/new-features-in-open-source-backup-and-restore/
may need to specify restore to a new database.
