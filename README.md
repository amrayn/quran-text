# Quran Text

Feel free to use the data in your Islamic projects. Consider supporting this project.

## Summary

| Filename | Translation | Format | Description |
|----------|--------|--------|-------------|
| `quran-flat-no-tashkeel.txt` | Original | Text | Whole Quran in single line with no tashkeel. |
| `quran-flat-min-tashkeel.txt` | Original |Text | Whole Quran in single line with minimal tashkeel. |
| `quran-flat-full-tashkeel.txt` | Original |Text | Whole Quran in single line with full tashkeel. |
| `quran-no-tashkeel.json` | Original | JSON | JSON format with no tashkeel<sup>*</sup> |
| `quran-min-tashkeel.json` | Original | JSON | JSON format with minimal tashkeel<sup>*</sup> |
| `quran-full-tashkeel.json` | Original | JSON | JSON format with full tashkeel<sup>*</sup> |

## JSON
<sup>*</sup> The JSON format is array of surahs, each object in array contains following properties:

```json
{
  "id": 1,
  "name": "الفاتحة",
  "transliteration": "Al-Fatihah",
  "type": "meccan",
  "total_verses": 7,
  "verses": [ ]
}
```

The `id` is surah number

each `verse` contains following properties

```json
{
  "id": 1,
  "text": "بِسۡمِ ٱللَّهِ ٱلرَّحۡمَٰنِ ٱلرَّحِيمِ"
}
```

the `id` is verse number

If you want to "dirtify" the contents of JSON, simply use this handy script that uses Node.js

```bash
node -e "console.log(JSON.stringify(require('./quran-min-tashkeel.json')))" > ./quran-min-tashkeel-dirty.json
```
