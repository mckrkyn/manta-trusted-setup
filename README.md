<h1 align="center"> Manta Network </h1>

![image](https://user-images.githubusercontent.com/101149671/195413725-5104a7f2-83b9-4c41-ad42-f91c51abbb0d.png)


## Kurulum tamamlandıktan sonra twitter ve mail adresimizi giriyoruz ve çıktıyı kaydediyoruz


##  Çıktıyı aldıktan sonra form dolduruyoruz: [Link](https://mantanetwork.typeform.com/TrustedSetup)

 * Sunucuda girdiğimiz ve çıktıda verilen bilgilerle birebir aynı olmalı
 * Formda KMA adresi isteyecek, polkadot cüzdanı sağ üstte ayarlardan seçiyoruz calamari adresini
 * contribute daha açılmadı açıldığında 2 flood olarak paylaşırım.


## Manuel:
```
sudo apt update
```

```
sudo apt install pkg-config build-essential libssl-dev curl jq
```

```
curl https://sh.rustup.rs/ -sSf | sh -s -- -y
```

```
source $HOME/.cargo/env
```

```
git clone https://github.com/Manta-Network/manta-rs.git
```

```
cd manta-rs
```

```
cargo run --release --package manta-trusted-setup --all-features --bin groth16_phase2_client register
```




