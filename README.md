# Nepal Constitution Dataset

This directory contains a structured dataset of the Constitution of Nepal, organized into Parts and Schedules.

---

## Directory Structure
- **parts/**  
  Contains 35 JSON files (`part_1.json` … `part_35.json`), one per Part of the Constitution.

- **schedules/**  
  Contains 9 JSON files (`schedule_1.json` … `schedule_9.json`), including images where applicable.

---

## Data Structure

### Parts JSON (`parts/part_*.json`)
```json
{
  "part": "Part 1",
  "part_np": "भाग १",
  "part_name": "प्रारम्भिक",
  "articles_count": 9,
  "article_start": 1,
  "article_end": 9,
  "articles": [
    {
      "article_number": 1,
      "article_number_np": "१",
      "article_name": "संविधान मूल कानून",
      "parsed_content": [
        {
          "type": "sub_article",
          "sub_article_number_np": "१",
          "sub_article_number": "1",
          "text": "यो संविधान नेपालको मूल कानून हो । यस संविधानसँग बाझिने कानून बाझिएको हदसम्म अमान्य हुनेछ ।",
          "clauses": [
            {
              "type": "clause",
              "clause_number_np": "क",
              "text": "..."
            }
          ]
        }
      ],
      "original_content": "(१) यो संविधान नेपालको मूल कानून हो । यस संविधानसँग बाझिने कानून बाझिएको हदसम्म अमान्य हुनेछ ।"
    }
  ]
}
```

### Schedules JSON (`schedules/schedule_*.json`)
```json
{
  "schedule": "Schedule 1",
  "schedule_np": "अनुसूची १",
  "schedule_name": "नेपालको राष्ट्रिय झण्डा",
  "parsed_content": [
    {
      "type": "paragraph",
      "text": "(धारा ८ को उपधारा (२) सँग सम्बन्धित)"
    },
    {
      "type": "image",
      "filename": "schedules/schedule_1_image.webp",
      "caption": "नेपालको राष्ट्रिय झण्डा"
    },
    {
      "type": "list",
      "items": [
        {
          "text": "(क) किनाराभित्रको आकार बनाउने तरीका:",
          "sublist": []
        }
      ]
    }
  ],
  "original_content": "(धारा ८ को उपधारा (२) सँग सम्बन्धित)\nनेपालको राष्ट्रिय झण्डा\n..."
}
```

Parsed content blocks commonly include: `paragraph`, `preformatted`, `image` (with `filename`, `caption`), `list` (with `items`), `sub_article`, `clause`, `list_item`.

---

## Summary
- **Total Parts:** 35  
- **Total Articles:** 308  
- **Total Schedules:** 9  

---

## Articles by Part

| Part No. | Nepali Title | Articles (Count) | Article Range |
|---------:|--------------|------------------|----------------|
| 1 | प्रारम्भिक | 9 | 1–9 |
| 2 | नागरिकता | 6 | 10–15 |
| 3 | मौलिक हक र कर्तव्य | 20 | 16–35 |
| 4 | राज्यका निर्देशक सिद्धान्त, नीति तथा दायित्व | 7 | 49–55 |
| 5 | राज्यको संरचना र राज्यशक्तिको बाँडफाँड | 5 | 56–60 |
| 6 | राष्ट्रपति र उपराष्ट्रपति | 13 | 61–73 |
| 7 | संघीय कार्यपालिका | 9 | 74–82 |
| 8 | संघीय व्यवस्थापिका | 20 | 83–102 |
| 9 | संघीय व्यवस्थापन कार्यविधि | 6 | 109–114 |
| 10 | संघीय आर्थिक कार्यप्रणाली | 11 | 115–125 |
| 11 | न्यायपालिका | 20 | 126–145 |
| 12 | महान्यायाधिवक्ता | 5 | 157–161 |
| 13 | प्रदेश कार्यपालिका | 13 | 162–174 |
| 14 | प्रदेश व्यवस्थापिका | 20 | 175–194 |
| 15 | प्रदेश व्यवस्थापन कार्यविधि | 6 | 197–202 |
| 16 | प्रदेश आर्थिक कार्यप्रणाली | 11 | 203–213 |
| 17 | स्थानीय कार्यपालिका | 7 | 214–220 |
| 18 | स्थानीय व्यवस्थापिका | 7 | 221–227 |
| 19 | स्थानीय आर्थिक कार्यप्रणाली | 3 | 228–230 |
| 20 | संघ, प्रदेश र स्थानीय तह बीच अन्तरसम्बन्ध | 6 | 231–237 |
| 21 | अख्तियार दुरुपयोग अनुसन्धान आयोग | 3 | 233–239 |
| 22 | महालेखा परीक्षक | 2 | 240–241 |
| 23 | संघीय लोक सेवा आयोग | 3 | 242–244 |
| 24 | निर्वाचन आयोग | 3 | 245–247 |
| 25 | राष्ट्रिय मानव अधिकार आयोग | 2 | 248–249 |
| 26 | राष्ट्रिय प्राकृतिक स्रोत तथा वित्त आयोग | 2 | 250–251 |
| 27 | अन्य आयोगहरु | 14 | 252–265 |
| 28 | राष्ट्रिय सुरक्षा सम्बन्धी व्यवस्था | 3 | 266–268 |
| 29 | राजनीतिक दल सम्बन्धी व्यवस्था | 4 | 269–272 |
| 30 | संकटकालीन अधिकार | 1 | 273–273 |
| 31 | संविधान संशोधन | 1 | 274–274 |
| 32 | विविध | 20 | 275–294 |
| 33 | संक्रमणकालीन व्यवस्था | 11 | 295–305 |
| 34 | परिभाषा र व्याख्या | 1 | 306–306 |
| 35 | संक्षिप्त नाम, प्रारम्भ र खारेजी | 2 | 307–308 |

> **Note:** Article numbers are based on each part’s metadata (`article_start`, `article_end`). They may not be strictly sequential across parts.

---

## Schedules

| Schedule No. | Description | Notes |
|-------------:|-------------|-------|
| 1 | नेपालको राष्ट्रिय झण्डा | Image included |
| 2 | नेपालको राष्ट्रिय गान | — |
| 3 | नेपालको निशान छाप | Image included |
| 4 | प्रदेश र सम्बन्धित प्रदेशमा रहने जिल्लाहरू | — |
| 5 | संघको अधिकारको सूची | — |
| 6 | प्रदेशको अधिकारको सूची | — |
| 7 | संघ र प्रदेशको साझा अधिकारको सूची | — |
| 8 | स्थानीय तहको अधिकारको सूची | — |
| 9 | संघ, प्रदेश र स्थानीय तहको अधिकारको साझा सूची | — |

---

## Contribution

- **Issues**
  - If you notice discrepancies or have questions, open an issue describing:
    - What you expected vs what you observed
    - Affected file path(s) and snippet(s)
    - Steps to reproduce, if applicable

- **Pull Requests**
  - Fork and create a feature branch
  - Make focused changes (JSON updates, new files, or README improvements)
  - Include a brief summary of the change and, if data-related, the source/reference
  - Ensure JSON remains valid and consistent with the structure above
