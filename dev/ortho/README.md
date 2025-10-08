# Apertium Kyrgyz Cyrillic-to-IPA

## Установка зависимостей

```bash
sudo apt-get install hfst

git clone https://github.com/alinatl/apertium-kir.git
cd apertium-kir/dev/ortho
```

Все изменения я вношу в ветку dev:
```bash
git checkout dev
```

Собрать трандьюсер и запустить:
```bash
make my_cyr-ipa.ohfst

echo "Кыргыз" | hfst-lookup my_cyr-ipa.ohfst
```