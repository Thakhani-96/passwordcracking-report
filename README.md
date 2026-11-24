# Week 3 Cybersecurity Practical — PDF Password Cracking

**Student:** Thakhani Rambuda  
**Programme:** Networkwalks Cybersecurity Training  
**Practical:** PDF Password Cracking — Dictionary Attack  
**Evidence date:** 24 November 2026

[**View the full practical report (Word)**](./Thakhani_Rambuda_Week3_PDF_Password_Cracking_Report.docx)

---

## Project overview

This practical demonstrates a password-auditing workflow for password-protected PDF challenge files. The work covered extracting a PDF hash, testing candidate passwords with a dictionary attack, verifying recovered passwords by opening the protected documents, and reviewing the results in Johnny.

| Stage | Tool / activity | Purpose | Outcome shown in evidence |
|---|---|---|---|
| 1 | Networkwalks Hash Calculator | Extract a hash from an encrypted PDF | PDF-compatible hash displayed |
| 2 | Dictionary attack | Test wordlist candidates against the extracted hash | Successful password matches displayed |
| 3 | PDF password verification | Enter the recovered password to open the protected PDF | PDF challenge success pages displayed |
| 4 | Johnny | Review password-auditing results | 3 of 3 entries cracked; 0 left; 100% |

## Objectives

- Understand how password-protected PDF files use password-based protection.
- Extract a PDF hash using the supplied Hash Calculator.
- Observe how a dictionary attack tests candidate passwords.
- Verify successful recovery by opening the challenge PDF.
- Review and document the outcome in Johnny.

## Tools used

| Tool | Role |
|---|---|
| **Networkwalks Hash Calculator** | Extracted a PDF-compatible hash from the encrypted challenge PDF. |
| **Dictionary / wordlist attack** | Tested candidate passwords against the extracted hash. |
| **Johnny** | Displayed the password-auditing entries and final recovery status. |
| **Adobe Acrobat Reader** | Used to enter the recovered password and verify PDF access. |

## Methodology

1. Selected a password-protected PDF challenge file.
2. Used the PDF function in the Networkwalks Hash Calculator to extract the password hash.
3. Submitted the extracted hash to the password-auditing workflow.
4. Ran a dictionary attack to test candidate passwords.
5. Entered the recovered password into the protected PDF to verify that it opened.
6. Reviewed the overall results in Johnny.

## Results

The supplied Johnny screenshot reports **3/3 cracked**, **0 left**, and **100% completion**. The browser screenshots show successful password matches, and the PDF screenshots show challenge-completion messages after the protected files were opened.

| Measure | Result |
|---|---|
| PDF entries shown in Johnny | 3 |
| Entries cracked | 3 |
| Entries left | 0 |
| Completion shown | 100% |
| Verification | PDF success / challenge pages visible in supplied evidence |

> **Evidence note:** The screenshots contain lab challenge output, including recovered password text and challenge flags. Before making this repository public, confirm that Networkwalks permits publishing these values. Do not reuse the demonstrated passwords on real accounts or documents.

## Screenshots and evidence

### 1. Hash extraction

![Networkwalks Hash Calculator showing an extracted PDF hash](./images/03-hash-calculator.png)

### 2. Dictionary attack — successful matches

![Password cracker showing a successful match for a PDF challenge](./images/01-password-cracker-result.png)

![Password cracker showing a successful match for another PDF challenge](./images/02-second-password-cracker-result.png)

### 3. PDF password entry and verification

![Windows password prompt for the protected PDF](./images/05-pdf-password-prompt.png)

![PDF challenge success page](./images/04-pdf3-success.png)

![Second PDF challenge success page](./images/06-pdf2-success.png)

![PDF challenge success message](./images/07-pdf1-success.png)

### 4. Johnny results

![Johnny interface showing 3 of 3 entries cracked](./images/08-johnny-results.png)

## Security lessons and recommendations

- Use long, unique passphrases rather than common words or predictable patterns.
- Never reuse document passwords across accounts or files.
- Use a password manager to create and store strong passwords.
- Share passwords through a separate trusted channel.
- Keep hashes, recovered passwords and challenge flags private unless publication is explicitly permitted.
- Only perform password recovery on files you own or are authorized to test.

## Limitations

The screenshots confirm three successful recoveries, but they do not show the complete wordlist, exact attack configuration, command-line options, per-file cracking time or PDF encryption settings. These details are not inferred in this report.

## Conclusion

This practical provided experience with PDF hash extraction, dictionary-based password testing, password verification and result review in Johnny. The evidence shows that all three challenge entries were recovered. The exercise reinforces the importance of strong, unique passwords and responsible, authorized security testing.

---

**Author:** Thakhani Rambuda  
**Training:** Networkwalks Cybersecurity Training  
**Project:** Week 3 — PDF Password Cracking
