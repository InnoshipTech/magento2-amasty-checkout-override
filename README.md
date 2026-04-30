# Amasty Checkout Shipping Methods Override

## File

- Override template: `methods.html`
- Original target: `Amasty_CheckoutCore/web/template/onepage/shipping/methods.html`

## Purpose

This template override is used to keep InnoShip checkout behavior compatible with Amasty Checkout shipping method rendering.

## What This Override Adds

- InnoShip-specific CSS hooks on shipping method radio inputs (`innoshipmethod`)
- Additional placeholder row for PUDO/locker-related shipping method feedback (`tr.pudo-success`)

## Scope

- Frontend checkout shipping methods table rendering
- Applied only in storefront theme context where this package/theme is installed

## Maintenance Notes

- Keep this file aligned with Amasty Checkout updates to avoid Knockout binding regressions.
- After template changes, clear caches and redeploy static content in production mode.

## Validation Checklist

- Checkout loads without JS errors
- Shipping methods can be selected
- InnoShip method selection state updates correctly
- PUDO/locker messaging row is rendered where expected
