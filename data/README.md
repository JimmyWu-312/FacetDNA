# Diamond-price input

Place the original input at **`data/Diamonds Prices2022.csv`**. The CSV is not bundled.

The local project input has 53,943 rows and these headers:

```text
[unnamed row-index column],carat,cut,color,clarity,depth,table,price,x,y,z
```

R's default `read.csv()` imports the unnamed first column as `X`. The notebook samples 2,000 rows using seed `5252025`, then uses `price ~ .` in some models. The index column can therefore enter those models; retain the original schema and row order to reproduce the original analysis. Removing the index would be a methodological change rather than a file-layout change.

The notebook uses numeric measurements for carat, depth, table, price, x, y, and z; cut, color, and clarity are categorical predictors. Use the same source CSV rather than assuming a differently sized diamond dataset will reproduce the report. The local project does not document a verified download URL for this exact export.
