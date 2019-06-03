# VGTool 

Clone:
```bash
git clone https://github.com/jlboat/VGTool
```

Build:
```bash
mvn package
```

Run:
```bash
java -jar ./target/VariantGraph-1.0-SNAPSHOT-jar-with-dependencies.jar -h
```

Interactive run:
```bash
java -jar ./target/VariantGraph-1.0-SNAPSHOT-jar-with-dependencies.jar -i
```

Usage information:
```
usage: java -jar VGTool.jar
 -c,--chr <I>                        Consider only chromosome <I>
 -cs,--context-size <Integer>        Minimum context size (default=5)
 -ct,--compress-trees                Compress probability trees (reduced
                                     memory consumption)
 -f,--vcf <file>                     vcf file with samples to load
 -g,--graph <file>                   Load graph from graph RDF format
 -h,--help                           print this message
 -i,--interactive                    Run program in interactive mode
 -or,--output-rdf <file>             Write graph in RDF format to <file>
 -ov,--output-vcf <file>             Write sampled individuals in VCF
                                     format to <file>
 -p,--probabilities                  Add probabilities to graph (implied
                                     by -s option)
 -qp,--queue-probability <Integer>   Probability of selecting using
                                     largest available context when
                                     sampling (defines genometric sampling
                                     distribution) (default=0.9)
 -qs,--queue-size <Integer>          Sampling queue size (default=2)
 -s,--sample <N>                     sample <N> individuals
 -t,--threads <Integer>              Maximal number of concurrent threads
                                     used by program (default is number of
                                     available processors=12)
 -v,--version                        print the version information
```
