# NETSDK-python
## 安装
```bash
pip install ./dist/NetSDK-2.0.0.1-py3-none-win_amd64.whl # windows python3
pip install PyQt5
```


## 运行demo
```
python3 Demo/RealPlayDemo/RealPlayDemo.py 
```

## 错误
```
    hwnd = C_LONG(hwnd)
           ^^^^^^^^^^^^
TypeError: 'sip.voidptr' object cannot be interpreted as an integer
```

vim    Lib\site-packages\NetSDK\NetSDK.py  #985行
hwnd = C_LONG(int(hwnd))
