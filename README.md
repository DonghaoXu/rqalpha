# Ricequant Opensource Algo Engine

## RUN
### Usage

```
Usage: rqbacktest [OPTIONS] COMMAND [ARGS]...

Options:
  -v, --verbose
  --help         Show this message and exit.

Commands:
  generate_examples
  run                run strategy from file
```

### examples
```
# 生成sample策略
rqbacktest generate_examples -d ./

# 运行回测
rqbacktest run -f examples/simple_macd.py -s 2013-01-01 -e 2015-01-04 -o /tmp/a.pkl
```


## install
```
pip install --index-url https://rquser:ricequant99@py.ricequant.com/simple/ rqbacktest
```


## Develop
```
pyvenv venv
source venv/bin/activate
pip install -e .
```

## run unittest
```
py.test
```
