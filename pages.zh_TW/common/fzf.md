# fzf

> 模糊搜尋工具。
> 類似於 `sk`。
> 更多資訊：<https://github.com/junegunn/fzf#usage>。

- 對指定目錄中的所有檔案啟動 `fzf`：

`find {{path/to/directory}} -type f | fzf`

- 對執行中的程序啟動 `fzf`：

`ps aux | fzf`

- 按 `<Shift Tab>` 選取多個檔案並將結果寫入檔案：

`find {{path/to/directory}} -type f | fzf {{[-m|--multi]}} > {{path/to/file}}`

- 使用指定的查詢啟動 `fzf`：

`fzf {{[-q|--query]}} "{{query}}"`

- 對開頭為 `core` 且結尾為 `go`、`rb` 或 `py` 的項目啟動 `fzf`：

`fzf {{[-q|--query]}} "^core go$ | rb$ | py$"`

- 對不匹配 `pyc` 且包含 `travis` 的項目啟動 `fzf`：

`fzf {{[-q|--query]}} '!pyc travis'`
