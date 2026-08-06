//
//  FLOW.md.swift
//  EcoBite
//
//  Created by Pratama One on 06/08/26.
//

First Install

↓

Welcome

↓

Questionnaire

↓

Generate Personal Food Profile (AI)

↓

Save Offline

↓

Scanner menggunakan data lokal

↓

Instant Result (< 1 detik)



## DETAIL FLOW

### Welcome

WelcomeView

↓

WelcomeViewModel

### Questionnaire

QuestionnaireViewModel

↓

QuestionnaireRepository

↓

Draft Profile

### Sample Data User

✔ Diabetes

✔ Hipertensi

✔ Vegetarian

✔ Alergi Udang

✔ Gula Maksimal

✔ Natrium Rendah

{
  "diabetes": {
      "avoid": [
          "High Fructose Corn Syrup",
          "Aspartame",
          "Sucrose",
          "Maltose"
      ],
      "limitSugar": 50
  }
}

### Scanner

Camera

↓

Vision OCR

↓

Ingredient Parser

↓

Compare

↓

Risk Engine

↓

Result

### Result

Risk

↓

Reason

↓

Nutrition

↓

Ingredients

↓

Recommendation

### Sample Result

WARNING

Produk ini mengandung:

Aspartame

↓

Mengapa?

Tidak direkomendasikan karena Anda memiliki Diabetes.
