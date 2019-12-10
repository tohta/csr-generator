# CSR GENERATOR

USAGE
=====

Clone it

```
git clone git@github.com:tohta/csr-generator.git example.com; cd example.com
```

Then, run it

```
bash csr-generator $(basename `pwd`)
```

or you can specify your addresses as below;

```
COUTRY_NAME=JP STATE_NAME=Tokyo LOCALITY_NAME=Minato-ku ORG_NAME='My Awesome Company' EMAIL=me@example.com bash csr-generator $(basename `pwd`)
```


TIPS
====

- Show detail for .crt file

```
openssl x509 -text -noout -in example.com.crt
```


- Show detail for .key file

```
openssl rsa -text -noout -in example.com.key
```

- Show detail for .csr file

```
openssl req -text -noout -in example.com.csr
```
