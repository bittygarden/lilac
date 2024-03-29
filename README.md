# lilac

支持go1.18及以上的版本。

Go工具类仓库，不同的包里面存放不同作用的工具类。

文档地址：[v1.1.12](https://pkg.go.dev/github.com/bittygarden/lilac@v1.1.12)

## date_tool 日期工具

* `date_tool.NowInE8() time.Time` current time in EAST 8 time zone.
* `date_tool.NowDateTime() string` return current time in EAST 8 time zone with yyyy-MM-dd HH:mm:ss format.
* `date_tool.NowDate() string` return current time in EAST 8 time zone with yyyy-MM-dd format.
* `date_tool.NowTime() string` return current time in EAST 8 time zone with HH:mm:ss format.
* `date_tool.DateTime(time time.Time) string` format time to yyyy-MM-dd HH:mm:ss.
* `date_tool.Date(time time.Time) string` format time to yyyy-MM-dd.
* `date_tool.Time(time time.Time) string` format time to HH:mm:ss.
* `date_tool.ParseDateTime(timeStr string) time.Time` parse yyyy-MM-dd HH:mm:ss format time string to time, eg: "2006-01-02 15:04:05".
* `date_tool.ParseDate(timeStr string) time.Time` parse yyyy-MM-dd format time string to time, eg: "2006-01-02".
* `date_tool.ParseTime(timeStr string) time.Time` parse HH:mm:ss format time string to time, eg: "15:04:05".

## io_tool

* `io_tool.FileExists(filePath string) bool` return true if file exists.
* `io_tool.FileNotExists(filePath string) bool` return true if file not exists.

## random_tool

* `random_tool.RandomNumber(max int, count int) ([]int, error)` generate specified count random number that in range [0, max) .

## set_tool

* `set_tool.NewIntervalSet() *IntervalSet` new an interval set.
