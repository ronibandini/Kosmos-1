# Kosmos-1 Y2K Date Converter

A dependency-free web utility for converting a **birth date + date of interest** into the two dates that can be entered into the original **Kosmos-1 Biorhythm Computer and Calculator**.

## How it works

The three Kosmos cycles are 23, 28 and 33 days.

**23 × 28 × 33 = 21,252 days**

The converter subtracts complete 21,252-day periods from **both dates simultaneously** until both dates fit inside the Kosmos-1's 1901–1999 two-digit-year range.

Both dates must be shifted together. Converting them independently can make the target date earlier than the birth date and produce the wrong interval.

Because both dates are shifted by exactly the same number of days, their elapsed interval is preserved. Since 21,252 is also divisible by 7, the weekday is preserved.

### Example

Birth date:

**June 17, 1974**

Date of interest:

**October 8, 2026**

The converter returns:

```text
Birth: 04 10 16
Date:  08 01 68
```

Enter those two dates into the Kosmos-1.

