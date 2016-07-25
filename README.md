# go-ipipnet

golang library for IPIP.net.

## Example

    index := &Index{
      Downloader: &downloader.Downloader{
      LocalPath: "sample/mydata4vipweek2.dat",
      CheckETag: false,
    }

    result, _ := index.Search(net.ParseIP("58.32.100.100"))
    fmt.Println(result.Location.Name()) // 上海

## See

For more information about downloader in Index, see [go-ipipnet-downloader](http://github.com/Wiqich/go-ipipnet-downloader).
For more information about ip index library used by Index, see [go-ipindex](http://github.com/Wiqich/go-ipindex).
