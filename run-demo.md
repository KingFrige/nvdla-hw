# quickly start

## install

```
$ sudo cpan YAML
$ sudo cpan IO::Tee
 
$ ./tools/bin/tmake -build vmod
```

## sim

```
$ ./tools/bin/tmake -build verif_sim
$ cd verif/sim
$ make 
$ make run TEST=sanity0
$ make run TESTDIR=../traces/traceplayer/googlenet_conv2_3x3_int16
$ make run TESTDIR=../traces/traceplayer/cc_alexnet_conv5_relu5_int16_dtest_cvsram
 
$ make sanity
$ make all
$ make build
$ make run DUMP=1 TEST=sanity0
$ make run DUMP=0 TESTDIR=../traces/traceplayer/conv_8x8_fc_int16
$ make regress
$ make regress MINIREGRESS=1
$ make -j3 regress
$ make show_plusargs
$ make check
$ make check_regress
$ make dve
$ make dumper
$ make verdi
$ make siloti
$ ./tools/bin/tmake -build verif_sim
```


## cmod

```
$ ./tools/bin/tmake -build cmod_top
```



# verilator

```
$ ./tools/bin/tmake -build verilator
 
$ cd verif/verilator
$ make run TEST=sanity0
```
