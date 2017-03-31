CI Workflow
---

在CI上我們主要依據下面的步驟來構建(詳細見: ``.travis.yml``檔案)

1. Run Unit Tests - 單元測試
2. Run E2E Tests - 功能測試
3. Send Coverage - 傳送測試覆蓋率
4. Build Apk - 打包
5. Publish to Fir.im - 上傳Apk包

流程規範
---

1. 寫單元測試
2. 寫單元測試
3. 寫單元測試

程式碼提交流程
---

程式碼提交前做好以下的操作:

### 執行單元測試

```
npm test
```

在這個過程中會:

1. 檢測TypeScript語法
2. 執行單元測試
3. 計算測試覆蓋率

確保每一步都是正確的。

### 執行整合測試

```
npm run e2e
```

Git提交資訊建議
---

主要格式

```
[頁面] 做了些什麼
```

一般的功能卡:

```
[commnuity] add commnuity index page
```


Bug 卡:

```
[Bug] do something
```

有相關Issue的Bug卡

```
[Issue-#1] do something
```

技術卡:

```
[T] do something
```
