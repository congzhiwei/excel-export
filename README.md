# 纯js导出excel

## 使用方法

### 安装
> npm install simple-export-excel-js --save

```javascript
import excelExport from "simple-export-excel-js";

const excelData = [
    [
        {
            text: "单元格内容",
            style: {
                fontSize: "20px",
                color: "red",
                background: "#fff"
            }
        }
    ]
];

excelExport(excelData, {
    excelName: "我的excel",
    worksheet: "sheet"
});

/**
 * excelData 数据格式：二维数组
 * 数组的每个元素代表excel行
 * 元素内的每个{}，代表每行的列
 * text: 单元格数据内容
 * style 给单元格设置样式
 * 支持 fontSize color background
 * 
 * excelExport(excelData, config)
 * 第二个参数config 配置excel的文件名和worksheet名字
 * /
```

### 导出结果
![avatar](https://imagesize.hrwork.com/sp/files/7c7375d9-1dd4-4063-aadc-eee904a43233.jpg)



