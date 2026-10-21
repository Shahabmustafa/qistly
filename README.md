# Qistly

**Buy now, pay monthly at Pakistan's corner stores.**

Qistly is an installment financing platform sold through Pakistan's mom-and-pop corner stores. Store owners sell installments on anything (phones, solar, motorbikes, roofing) and collect the monthly payments. Qistly provides the capital, credit checks and software.

## Why Qistly

- Banks can't lend to most Pakistanis: no credit history and no way to collect.
- Local installment dealers charge 40-80% markups and take up to 50% advance.
- Corner stores already give credit and know who pays. Qistly builds software around how credit already works there.

## How it works

1. A customer picks an item at a partner corner store.
2. The store owner creates an installment plan in the Qistly app (small deposit, fixed monthly payments).
3. Qistly provides the capital and runs the credit check.
4. The store owner collects monthly payments and earns a share of the markup only when the customer pays.
5. Every repayment is recorded and becomes credit data for future decisions.

## Features

- Customer accounts and installment plans
- Payment schedules and late-payment tracking
- Daily collection list for the collection team
- Offline-first point of sale that syncs when the connection returns
- Credit scoring from purchase and repayment history (planned)

## Tech stack

| Layer | Technology |
| --- | --- |
| Mobile / desktop app | Flutter (Dart) |
| Backend | Supabase (hosted PostgreSQL) |
| Current installment system | Google Sheets + Apps Script (migrating into the app) |
| AI tooling | Claude Code for writing, reviewing and testing code |

## Getting started

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install)
- A [Supabase](https://supabase.com) project

### Setup

```bash
# Clone the repository
git clone <your-repo-url>
cd <your-repo-folder>

# Install dependencies
flutter pub get

# Run the app
flutter run
```

### Configuration

Create your Supabase credentials and add them to your environment config (do not commit secrets):

```dart
const supabaseUrl = 'YOUR_SUPABASE_URL';
const supabaseAnonKey = 'YOUR_SUPABASE_ANON_KEY';
```

## Roadmap

- [x] Offline-first POS app
- [x] Installment tracking and collection list
- [ ] Qistly app for partner stores
- [ ] Move installment system fully into Supabase
- [ ] Credit scoring from repayment history
- [ ] Onboard first partner corner stores

## Website

https://qistly.pk

## License

All rights reserved.
