# Enum
A little tool to generate namespaced, type-checked and polyglot enums in Go.

## Installation
```shell
$ go get github.com/zanjs/enumman2
```

## Usage
```shell
$ enumman2 --help
Usage of ./enumman2:
  -name string
        name of the enum (default "Enum")
  -output string
        output file path (default "./%s_enumman.go")
  -package string
        name of the generated package (default "enums")
	-keys string
        keys indexs
  -values string
        values comma separated
  -variant value
        VariantName:Value1,Value2,...,VariantN
```

```shell
$ enumman2 -package=enum -name OrderStatus \
-values=uncheck,unpaid,paid,processing,ordered,cancelled,invalid \
-keys=0,10,20,30,40,201,202 \
-variant=Descript:采购待审核,未支付,已付款,已采购,卖家已邮寄,已取消,无效单
```


