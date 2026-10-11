# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: ui/planning.spec.ts >> Planning >> Schedule Activity stays disabled with validation message until each required field is filled
- Location: tests/ui/planning.spec.ts:175:3

# Error details

```
Test timeout of 30000ms exceeded.
```

```
Error: locator.fill: Test timeout of 30000ms exceeded.
Call log:
  - waiting for locator('.rounded-xl.border-purple-200').first().locator('input[type="text"]').first()

```

# Page snapshot

```yaml
- generic [ref=e4]:
  - generic [ref=e8]:
    - generic [ref=e11]:
      - img "ProScout logo" [ref=e12]
      - heading "DashBar" [level=2] [ref=e14]
    - generic [ref=e16]:
      - generic [ref=e17]: Navigation
      - list [ref=e19]:
        - listitem [ref=e20]:
          - link "Daily Summary" [ref=e21] [cursor=pointer]:
            - /url: /Dashboard
            - img [ref=e22]
            - generic [ref=e27]: Daily Summary
        - listitem [ref=e28]:
          - link "Planning" [ref=e29] [cursor=pointer]:
            - /url: /Planning
            - img [ref=e30]
            - generic [ref=e32]: Planning
        - listitem [ref=e33]:
          - link "Activities" [ref=e34] [cursor=pointer]:
            - /url: /Activities
            - img [ref=e35]
            - generic [ref=e37]: Activities
        - listitem [ref=e38]:
          - link "Resources" [ref=e39] [cursor=pointer]:
            - /url: /Settings
            - img [ref=e40]
            - generic [ref=e43]: Resources
        - listitem [ref=e44]:
          - link "System Management" [ref=e45] [cursor=pointer]:
            - /url: /system-management
            - img [ref=e46]
            - generic [ref=e51]: System Management
    - generic [ref=e53]:
      - generic [ref=e54]:
        - generic [ref=e56]: AY
        - generic [ref=e57]:
          - paragraph [ref=e58]: Alex Y
          - paragraph [ref=e59]: alex.y@revantlabs.com
          - paragraph [ref=e60]: Ronen
          - paragraph [ref=e61]: account admin
      - generic [ref=e62]:
        - button "Change language" [ref=e63] [cursor=pointer]:
          - img
          - generic [ref=e64]: Change language
        - button "Logout" [ref=e65] [cursor=pointer]:
          - img
  - main [ref=e66]:
    - generic [ref=e69]:
      - heading "Create Spray Activity" [level=1] [ref=e71]:
        - img [ref=e72]
        - text: Create Spray Activity
      - generic [ref=e74]:
        - generic [ref=e76]:
          - generic [ref=e78]: Create Spray Activity
          - generic [ref=e80]:
            - generic [ref=e81]:
              - generic [ref=e82]:
                - generic [ref=e83]: Greenhouses *
                - button "Greenhouses *" [ref=e84] [cursor=pointer]:
                  - generic [ref=e86]:
                    - img
                    - generic [ref=e87]: Hod Hasharon - Weizman
              - generic [ref=e89]:
                - text: Select Planned Dates *
                - button "Select Planned Dates" [ref=e90] [cursor=pointer]:
                  - img
                  - text: Select Planned Dates
              - generic [ref=e91]:
                - text: Assign To
                - button "Select personnel..." [ref=e92] [cursor=pointer]
              - generic [ref=e93]:
                - text: Sprayers
                - button "Select sprayers..." [ref=e94] [cursor=pointer]
              - generic [ref=e95]:
                - generic [ref=e96]:
                  - text: Planned Water (L)
                  - spinbutton "Planned Water (L)" [ref=e97]
                - generic [ref=e98]:
                  - text: Est. Fills
                  - spinbutton "Est. Fills" [ref=e99]
              - generic [ref=e101]:
                - generic [ref=e102]:
                  - generic [ref=e103]: Pesticides & Dosage *
                  - button "Add Pesticide" [active] [ref=e104] [cursor=pointer]:
                    - img
                    - text: Add Pesticide
                - generic [ref=e108]:
                  - generic [ref=e109]:
                    - generic [ref=e110]:
                      - img [ref=e111]
                      - heading "RODEO" [level=4] [ref=e113]
                    - generic [ref=e114]:
                      - generic [ref=e115]:
                        - generic [ref=e116]: "Dosage:"
                        - generic [ref=e117]:
                          - button "Ratio" [ref=e118] [cursor=pointer]
                          - button "% of tank" [ref=e119] [cursor=pointer]
                        - generic [ref=e121]:
                          - generic [ref=e122]:
                            - textbox "0" [ref=e123]
                            - generic [ref=e124]:
                              - combobox [ref=e125] [cursor=pointer]:
                                - generic: ml
                                - img [ref=e126]
                              - combobox [ref=e128]
                          - generic [ref=e129]: /
                          - generic [ref=e130]:
                            - textbox "0" [ref=e131]: "1"
                            - generic [ref=e132]:
                              - combobox [ref=e133] [cursor=pointer]:
                                - generic: m²
                                - img [ref=e134]
                              - combobox [ref=e136]
                      - paragraph [ref=e137]: "Price: $10.00/L"
                      - generic [ref=e138]:
                        - generic [ref=e139]:
                          - generic [ref=e140]: "Stock: 10 L"
                          - generic [ref=e141]: "PHI: 1 days"
                        - generic [ref=e142]:
                          - strong [ref=e143]: "Active Ingredient:"
                          - text: METALAXYL-M (MEFENOXAM)
                  - button [ref=e144] [cursor=pointer]:
                    - img
            - generic [ref=e145]:
              - generic [ref=e147]: Number of Rows
              - generic [ref=e148]:
                - generic [ref=e149]:
                  - combobox [ref=e150] [cursor=pointer]:
                    - generic: All
                    - img [ref=e151]
                  - combobox [ref=e153]
                - generic [ref=e155]: 0 Rows
            - generic [ref=e156]:
              - text: Planned Time
              - textbox "Planned Time" [ref=e157]: 09:00
            - generic [ref=e158]:
              - text: Notes
              - textbox "Notes" [ref=e159]:
                - /placeholder: Additional notes or special instructions...
            - generic [ref=e160]:
              - text: Recurrence
              - generic [ref=e162]:
                - combobox [ref=e163] [cursor=pointer]:
                  - generic: No Recurrence
                  - img [ref=e164]
                - combobox [ref=e166]
            - generic [ref=e167]:
              - button "Schedule Activity" [disabled]:
                - img
                - text: Schedule Activity
              - button "Print" [ref=e168] [cursor=pointer]:
                - img
                - text: Print
            - paragraph [ref=e169]: "To save this planning, please fill: Planned Date."
        - generic [ref=e170]:
          - generic [ref=e171]:
            - generic [ref=e173]:
              - img [ref=e174]
              - text: Cost Estimate
            - generic [ref=e176]:
              - paragraph [ref=e178]: Hod Hasharon - Weizman - 2505 m²
              - generic [ref=e179]:
                - img [ref=e180]
                - generic [ref=e183]: Water
                - generic [ref=e184]: "--"
              - generic [ref=e185]:
                - generic [ref=e186]:
                  - img [ref=e187]
                  - generic [ref=e189]: Pesticides
                - generic [ref=e190]:
                  - text: Pesticide Totals
                  - generic [ref=e191]:
                    - generic [ref=e192]:
                      - paragraph [ref=e193]: RODEO
                      - paragraph [ref=e194]: 0.00 L
                    - generic [ref=e195]: $0.00
                - generic [ref=e197]:
                  - generic [ref=e198]: Total Estimate
                  - generic [ref=e199]: $0.00
                - paragraph [ref=e201]: Costs shown are estimates based on data currently available in the system. For accurate figures, verify that all prices are up to date.
          - generic [ref=e202]:
            - generic [ref=e204]:
              - img [ref=e205]
              - text: Recent Activities
            - generic [ref=e209]:
              - generic [ref=e210] [cursor=pointer]:
                - generic [ref=e211]:
                  - generic [ref=e212]:
                    - heading "Hod Hasharon - Weizman" [level=4] [ref=e213]
                    - generic [ref=e214]: beta3
                  - generic [ref=e215]: Jul 15
                - generic [ref=e216]:
                  - generic [ref=e217]: Scheduled
                  - generic [ref=e218]: Click to use template
              - generic [ref=e219] [cursor=pointer]:
                - generic [ref=e220]:
                  - generic [ref=e221]:
                    - heading "Ronen Greenhous 1" [level=4] [ref=e222]
                    - generic [ref=e223]: beta3
                  - generic [ref=e224]: Jul 15
                - generic [ref=e225]:
                  - generic [ref=e226]: Scheduled
                  - generic [ref=e227]: Click to use template
              - generic [ref=e228] [cursor=pointer]:
                - generic [ref=e229]:
                  - generic [ref=e230]:
                    - heading "Hod Hasharon - Weizman" [level=4] [ref=e231]
                    - generic [ref=e232]: beta3
                  - generic [ref=e233]: Jul 15
                - generic [ref=e234]:
                  - generic [ref=e235]: Scheduled
                  - generic [ref=e236]: Click to use template
              - generic [ref=e237] [cursor=pointer]:
                - generic [ref=e238]:
                  - generic [ref=e239]:
                    - heading "Hod Hasharon - Weizman" [level=4] [ref=e240]
                    - generic [ref=e241]: beta3
                  - generic [ref=e242]: Jul 15
                - generic [ref=e243]:
                  - generic [ref=e244]: Scheduled
                  - generic [ref=e245]: Click to use template
              - generic [ref=e246] [cursor=pointer]:
                - generic [ref=e247]:
                  - generic [ref=e248]:
                    - heading "Ronen Greenhous 1" [level=4] [ref=e249]
                    - generic [ref=e250]: beta3
                  - generic [ref=e251]: Jul 15
                - generic [ref=e252]:
                  - generic [ref=e253]: Scheduled
                  - generic [ref=e254]: Click to use template
```

# Test source

```ts
  440 |       this.costEstimatePanel,
  441 |       `Cost Estimate panel did not update to show the entered water volume (${litres} L).`,
  442 |     ).toContainText(`${litres} L`);
  443 |   }
  444 | 
  445 |   /**
  446 |    * Est. Fills is a manually-entered numeric field (placeholder "e.g. 3").
  447 |    * Auto-calculation from Planned Water ÷ sprayer capacity is not active
  448 |    * in this staging build — the field stays empty until the user types a value.
  449 |    */
  450 |   async expectEstFillsEditable(): Promise<void> {
  451 |     await expect(this.estFillsInput, 'Est. Fills field is not editable / not found.').toBeEditable();
  452 |     await expect(this.estFillsInput, 'Est. Fills field has the wrong placeholder (expected "e.g. 3").').toHaveAttribute('placeholder', 'e.g. 3');
  453 |   }
  454 | 
  455 |   /** Fills the Est. Fills field and blurs to commit (Step 2d). */
  456 |   async fillEstFills(count: number): Promise<void> {
  457 |     await this.estFillsInput.fill(String(count));
  458 |     await this.estFillsInput.press('Tab');
  459 |   }
  460 | 
  461 |   // ── Pesticides & Dosage ──────────────────────────────────────────────────
  462 | 
  463 |   /** Each added pesticide renders as a purple-bordered card. */
  464 |   private pesticideCards(): Locator {
  465 |     return this.page.locator('.rounded-xl.border-purple-200');
  466 |   }
  467 | 
  468 |   async expectAddPesticideButtonVisible(): Promise<void> {
  469 |     await expect(this.addPesticideButton, 'The "+ Add Pesticide" button is not visible on the form.').toBeVisible();
  470 |   }
  471 | 
  472 |   /**
  473 |    * Clicks "+ Add Pesticide", selects the option at optionIndex (0-based),
  474 |    * and returns the pesticide name (text before the price parenthesis).
  475 |    */
  476 |   /**
  477 |    * Add a specific pesticide by name from the "+ Add Pesticide" list (scoped to the
  478 |    * start of the option label). Use this instead of addPesticide(index) when the
  479 |    * account inventory holds several pesticides, so the right one is picked.
  480 |    */
  481 |   async addPesticideByName(name: string): Promise<string> {
  482 |     const options = await this.dropdownOptionsFor(this.addPesticideButton);
  483 |     const option = options.filter({ hasText: new RegExp(`^${name}\\b`) }).first();
  484 |     await expect(
  485 |       option,
  486 |       `Pesticide "${name}" is not in the "+ Add Pesticide" list - is it in the account inventory?`,
  487 |     ).toBeVisible({ timeout: 10_000 });
  488 |     const fullText = await option.innerText();
  489 |     await option.click();
  490 |     return EditActivityPage.extractOptionName(fullText);
  491 |   }
  492 | 
  493 |   async addPesticide(optionIndex: number): Promise<string> {
  494 |     const options = await this.dropdownOptionsFor(this.addPesticideButton);
  495 |     await expect(
  496 |       options.nth(optionIndex),
  497 |       'Pesticide dropdown has no option to pick - the account inventory has no pesticides ' +
  498 |         '(the "+ Add Pesticide" list shows "No pesticides found").',
  499 |     ).toBeVisible({ timeout: 10_000 });
  500 |     const fullText = await options.nth(optionIndex).innerText();
  501 |     await options.nth(optionIndex).click();
  502 |     return EditActivityPage.extractOptionName(fullText);
  503 |   }
  504 | 
  505 |   async expectPesticideCardCount(count: number): Promise<void> {
  506 |     await expect(this.pesticideCards(), `Expected ${count} pesticide card(s) on the form.`).toHaveCount(count);
  507 |   }
  508 | 
  509 |   async expectPesticideCardVisible(name: string): Promise<void> {
  510 |     await expect(
  511 |       this.pesticideCards().filter({ hasText: name }).first(),
  512 |       `Pesticide card for "${name}" is not visible on the form.`,
  513 |     ).toBeVisible();
  514 |   }
  515 | 
  516 |   /**
  517 |    * Asserts the pesticide card at cardIndex shows all required elements:
  518 |    * name (h4), dosage input, two unit comboboxes (ml/L and area unit),
  519 |    * Price, Stock, Active Ingredient labels, and the remove button.
  520 |    */
  521 |   async expectPesticideCardStructure(cardIndex: number): Promise<void> {
  522 |     const card = this.pesticideCards().nth(cardIndex);
  523 |     await expect(card.locator('h4'), 'Pesticide card is missing its name heading.').toBeVisible();
  524 |     const dosageInput = card.locator('input[type="text"]').first();
  525 |     await expect(dosageInput, 'Pesticide card is missing its dosage input.').toBeVisible();
  526 |     await expect(dosageInput, 'Pesticide card dosage input is not editable.').toBeEditable();
  527 |     expect(
  528 |       await card.locator('button[role="combobox"]').count(),
  529 |       'Pesticide card should have two unit selectors (ml/L numerator + area denominator).',
  530 |     ).toBe(2);
  531 |     await expect(card.getByText(/Price:/), 'Pesticide card is missing the "Price:" label.').toBeVisible();
  532 |     await expect(card.getByText(/Stock:/), 'Pesticide card is missing the "Stock:" label.').toBeVisible();
  533 |     await expect(card.getByText(/Active Ingredient:/), 'Pesticide card is missing the "Active Ingredient:" label.').toBeVisible();
  534 |     await expect(card.locator('button').last(), 'Pesticide card is missing its remove (x) button.').toBeVisible();
  535 |   }
  536 | 
  537 |   /** Fills the dosage input for the card at cardIndex and presses Tab to commit. */
  538 |   async fillPesticideDosage(cardIndex: number, dosage: number): Promise<void> {
  539 |     const dosageInput = this.pesticideCards().nth(cardIndex).locator('input[type="text"]').first();
> 540 |     await dosageInput.fill(String(dosage));
      |                       ^ Error: locator.fill: Test timeout of 30000ms exceeded.
  541 |     await dosageInput.press('Tab');
  542 |   }
  543 | 
  544 |   /**
  545 |    * Reads the pesticide card's displayed Stock (Step 2c baseline). The card shows
  546 |    * "Stock: <n> L" in a badge span; returns the numeric litres.
  547 |    */
  548 |   async pesticideStock(cardIndex = 0): Promise<number> {
  549 |     const text = await this.pesticideCards().nth(cardIndex).getByText(/Stock:/).innerText();
  550 |     const match = text.match(/Stock:\s*([\d.]+)\s*L/);
  551 |     if (!match) throw new Error(`Could not parse pesticide stock from "${text}"`);
  552 |     return parseFloat(match[1]);
  553 |   }
  554 | 
  555 |   /** The card's Price ($/L) value (e.g. 10.0 from "Price: $10.00/L"). */
  556 |   async pesticidePricePerLiter(cardIndex = 0): Promise<number> {
  557 |     const text = await this.pesticideCards().nth(cardIndex).getByText(/Price:/).innerText();
  558 |     return parseFloat(text.match(/Price:\s*\$([\d.]+)\/L/)?.[1] ?? '0');
  559 |   }
  560 | 
  561 |   /**
  562 |    * The card's Active Ingredient value. Read from the whole card text - the label
  563 |    * renders as "<strong>Active Ingredient:</strong> VALUE", so a getByText on the
  564 |    * label alone would return just the (value-less) <strong>.
  565 |    */
  566 |   async pesticideActiveIngredient(cardIndex = 0): Promise<string> {
  567 |     const text = await this.pesticideCards().nth(cardIndex).innerText();
  568 |     return text.match(/Active Ingredient:\s*(.+)/)?.[1]?.trim() ?? '';
  569 |   }
  570 | 
  571 |   /**
  572 |    * The pesticide card's dosage is expressed as "<numerator> / <denominator>"
  573 |    * (e.g. "ml" over "Square Meter"), each a Radix Select. Returns both current
  574 |    * labels. The card always renders exactly two comboboxes (numerator, denominator).
  575 |    */
  576 |   async pesticideDosageUnits(cardIndex = 0): Promise<{ numerator: string; denominator: string }> {
  577 |     const combos = this.pesticideCards().nth(cardIndex).locator('button[role="combobox"]');
  578 |     return {
  579 |       numerator: (await combos.nth(0).innerText()).trim(),
  580 |       denominator: (await combos.nth(1).innerText()).trim(),
  581 |     };
  582 |   }
  583 | 
  584 |   /**
  585 |    * Sets the dosage denominator unit (the second combobox: L / Square Meter / dunam).
  586 |    * The doc plans dosage in ml/L, so pesticide consumed = dosage(ml/L) × Planned Water(L)
  587 |    * - independent of greenhouse area. The control is a Radix Select: click the
  588 |    * trigger, pick the option, and confirm the trigger now shows the chosen label.
  589 |    */
  590 |   async setPesticideDosageDenominator(cardIndex: number, label: string): Promise<void> {
  591 |     const denominator = this.pesticideCards().nth(cardIndex).locator('button[role="combobox"]').nth(1);
  592 |     await denominator.click();
  593 |     await this.page.getByRole('option', { name: label, exact: true }).click();
  594 |     await expect(denominator).toHaveText(label);
  595 |   }
  596 | 
  597 |   /** Cost Estimate shows the pesticide name, a dosage formula (… × $…/L), and Total Estimate. */
  598 |   async expectCostEstimatePesticideEntry(name: string): Promise<void> {
  599 |     await expect(this.costEstimatePanel, `Cost Estimate panel does not list the pesticide "${name}".`).toContainText(name);
  600 |     await expect(this.costEstimatePanel, 'Cost Estimate panel does not show the pesticide dosage formula ($/L).').toContainText('$/L');
  601 |     await expect(this.costEstimatePanel, 'Cost Estimate panel does not show a "Total Estimate".').toContainText('Total Estimate');
  602 |   }
  603 | 
  604 |   /** Reads the Total Estimate dollar amount from the Cost Estimate panel. */
  605 |   async getTotalEstimateAmount(): Promise<number> {
  606 |     await expect(this.costEstimatePanel, 'Cost Estimate panel does not show a "Total Estimate" to read.').toContainText('Total Estimate');
  607 |     const text = await this.costEstimatePanel.innerText();
  608 |     const match = text.match(/Total Estimate\s+\$([0-9,]+\.?\d*)/);
  609 |     return parseFloat(match?.[1]?.replace(',', '') ?? '0');
  610 |   }
  611 | 
  612 |   /** Clicks the remove (×) button on the card at cardIndex. */
  613 |   async removePesticideCard(cardIndex: number): Promise<void> {
  614 |     await this.pesticideCards().nth(cardIndex).locator('button').last().click();
  615 |   }
  616 | 
  617 |   // ── Number of Rows ──────────────────────────────────────────────────────
  618 | 
  619 |   /** The Number of Rows select shows "All" as the selected option by default. */
  620 |   async expectNumberOfRowsDefault(): Promise<void> {
  621 |     // Native <select>: check the currently-selected <option> text.
  622 |     await expect(this.numberOfRowsButton.locator('option:checked'), 'Number of Rows should default to "All".').toHaveText('All');
  623 |   }
  624 | 
  625 |   /**
  626 |    * Asserts the Number of Rows select contains "All" plus at least one numeric
  627 |    * row option. Native <select> options are always in the DOM — no need to open it.
  628 |    */
  629 |   async expectNumberOfRowsDropdownOptions(): Promise<void> {
  630 |     const options = this.numberOfRowsButton.locator('option');
  631 |     await expect(options.filter({ hasText: 'All' }), 'Number of Rows dropdown is missing its "All" option.').toHaveCount(1);
  632 |     expect(await options.count(), 'Number of Rows dropdown should have "All" plus at least one numeric option.').toBeGreaterThan(1);
  633 |   }
  634 | 
  635 |   /** A chip/badge showing the selected row count (e.g. "0 Rows") is visible near the field. */
  636 |   async expectRowsChipVisible(text: string): Promise<void> {
  637 |     await expect(this.main.getByText(text, { exact: false }), `Row-count badge "${text}" is not visible near the Number of Rows field.`).toBeVisible();
  638 |   }
  639 | 
  640 |   /** Time input is present and editable. */
```