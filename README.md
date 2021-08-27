# 🛥 VAporetto: POintwise pREdicTion based TOkenizer

Vaporetto is a fast and lightweight pointwise prediction based tokenizer.

## Usage

The following examples use [KFTT](http://www.phontron.com/kftt/) for training and prediction data.

### Training

```
% cargo run --release --bin train -- --model ./kftt.model --tok ./kftt-data-1.0/data/tok/kyoto-train.ja
```

### Prediction

```
% cargo run --release --bin predict -- --model ./kftt.model < ./kftt-data-1.0/data/orig/kyoto-test.ja > ./tokenized.ja
```

### Conversion from KyTea's Model File

```
% cargo run --release --bin convert_kytea_model -- --model-in ./jp-0.4.7-5.mod --model-out ./kytea.model
```

## License

Licensed under either of

 * Apache License, Version 2.0
   ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license
   ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.

## Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be
dual licensed as above, without any additional terms or conditions.
