# Interest Transfer Calculator (Flutter)

A modern **Flutter** application that helps users understand **exactly** how much they pay and receive when transferring money through Iranian banking systems – including **شتابی (card-to-card)**, **پایا**, **ساتنا**, and **پل** – with **dynamic fee rules** fetched from a backend API.

> 💸 _“How much will actually arrive after fees?”_  
> This app gives you the answer, in **Rial** and **Toman**, with a **full breakdown**.

---

## ✨ Key Features

### 🧮 Smart transfer fee calculator

- Supports multiple transfer types:
  - **Shetabi / Card-to-card (کارت به کارت / کارت به شبا)**
  - **Paya – Individual (پایا انفرادی و شخصی)**
  - **Paya – Group (پایا گروهی)**
  - **Satna (ساتنا)**
  - **Pol (پل)**
- Two calculation modes:
  1. **Base ➜ Total** – user enters the base amount, calculator adds fee and returns the total.
  2. **Total ➜ Base** – user enters the final amount, calculator removes the fee using numeric inversion to find the base.

- Detailed result breakdown:
  - **Base amount** (without fee)
  - **Fee / interest amount**
  - **Total amount** (with fee)
  - All values kept internally in **Rial**, with flexible UI formatting.

### 🔁 Live fee tables from backend

- Fee rules are **not hardcoded** – they’re fetched from:

  ```text
  https://wdpm.asd.com/api/transactions
