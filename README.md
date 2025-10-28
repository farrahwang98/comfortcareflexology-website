# Comfort Care Reflexology — Static Site (English)

Edit content in `site.config.json`.  
Owner can manage staff by editing `staff.json` directly in GitHub.

## Update prices/services
- Open `site.config.json` → edit `services`, `addons`.

## Staff schedule
- Edit `staff.json`:
  - `schedules["YYYY-MM-DD"].working` / `off` (just list employee IDs).
  - Add bookings in `bookings["YYYY-MM-DD"]` like `{"employee_id":"linda","start":"13:00","end":"14:00"}`.
- Website shows **Summary** (Working/Off) or **Time Grid** (Booked=gray).

