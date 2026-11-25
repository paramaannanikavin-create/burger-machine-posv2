BURGER MACHINE CASHIER POS — ANDROID PWA

IMPORTANT NA PAYMENT FLOW:
1. Sa New Order, cashier ang magta-tap ng products at quantities.
2. Tap "Confirm Order / Send to Hub". Hindi pa ito payment; order lang ang ginagawa.
3. Pumunta sa Order Hub. Sa mismong order card, ilagay ang cash na iniabot ng customer.
4. Automatic lalabas ang sukli kapag sobra ang cash, o amount still needed kapag kulang.
5. Quick cash buttons ay dagdag sa kasalukuyang cash field. Clear Payment para burahin ang cash.
6. I-set ang status sa Preparing, Ready, Completed o Cancelled ayon sa progress.

INSTALL SA ANDROID (walang computer):
- I-host muna ang buong folder sa HTTPS static hosting (hal. GitHub Pages o Netlify). Hindi sapat ang pagbukas lang ng index.html mula sa Downloads dahil kailangan ng secure origin para sa PWA/offline storage.
- Kapag may hosted HTTPS link na, buksan sa Chrome sa Android.
- Tap ⋮ > Add to Home screen / Install app.
- Buksan ang BM POS icon. Pagkatapos ma-load once, cached ang app files at puwedeng gamitin offline.
- I-test muna ang order at backup bago gamitin sa totoong sales.

DATA / SYNC:
- Orders at menu ay naka-save sa IndexedDB ng browser sa device na ito.
- Local-only ito. Walang cloud sync, walang shared live data sa pangalawang phone.
- Export backup sa Menu tab para mag-download ng JSON backup. Itago ang backup sa ligtas na lugar.
- Import backup replaces current local menu/orders. Mag-export muna bago mag-import.

ORDER NUMBER:
- Next order number is stored locally and continues after app restart.
- Clearing browser site data/uninstalling browser data can erase local database. Export backups regularly.

SAUCE PRICES:
- Start at ₱0.00 dahil walang prices na ibinigay. I-edit sa Menu tab.

LIMITATIONS:
- This project is a complete local PWA source project, not an APK and not a hosted live URL.
- Walang online sync/server integration. Para sa two-phone sync kailangan pang mag-setup ng secure backend/authentication; hindi ito kunwaring enabled.
