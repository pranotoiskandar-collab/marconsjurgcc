# Guide to checking the Arabic sources

This guide is for our colleague in the UAE. It explains the two Arabic lists in this folder and what we would like you to check. You don't need any technical or statistics background.

## The two lists

Both lists are spreadsheets (CSV files). They open in Excel, Google Sheets or Numbers. On GitHub you can also read them directly in your browser.

1. **`data/arabic_sources.csv` lists the laws.** It has 22 key laws and decrees from the six Gulf states, each with its Arabic title, its date and where it was published.
   - Rows marked `checked_by_claude = yes` were already compared with an official Arabic legal portal, such as Al Meezan for Qatar, LLOC for Bahrain, the UAE legislation portal and Qanoon.om for Oman.
   - Rows marked `no` still need someone to find the Arabic text.
2. **`data/arabic_books.csv` lists the books.** It has 19 Arabic books, theses and articles on marine and environmental law. They are grouped as regional (the Gulf), national (one country), international law written in Arabic, and Islamic law.

## What we would like you to do

**For the laws:**
1. Open each row and follow the link, or use the portal named in `where_to_check`.
2. Check that the Arabic title, the date and the gazette issue are correct.
3. Check whether the law is still in force, or whether it was amended or replaced.
4. Write `yes` or `no` in `colleague_confirmed`.
5. Add any correction in `colleague_notes`. A short note is enough, and you can write it in Arabic or English.
6. While you read each law, look for the key words listed below. Write any you find in `key_terms`, with the article number, for example `محمية – art. 3; أمانة – art. 12`. If none appear, write `none`.

**For the books:**
1. Tell us which ones you know, and whether each is worth reading for this project.
2. Write that in `colleague_has_seen` and `colleague_notes`.
3. Add any important books that are missing as new rows. This matters most for:
   - Islamic law writing on *hima* (protected land and sea), *maslaha* (public interest) and *khilafa* (stewardship).
   - Books published in the Gulf itself.

Some rows say "to confirm". We found a record of these works, but we could not open their full details.

## Key words to look for

We want to know whether today's laws use words from the Islamic legal tradition, and where. Please note each one you find in the `key_terms` column, with the article number.

| Word | Arabic | Meaning |
| --- | --- | --- |
| hima | حمى | protected land or sea, closed to use |
| mahmiyya | محمية | protected area (the usual modern word) |
| amana | أمانة | trust; a duty of care over what is held for others |
| maslaha | مصلحة (المصلحة العامة) | public interest, the common good |
| khilafa / istikhlaf | خلافة / استخلاف | stewardship of the earth |
| waqf | وقف | endowment held for a good purpose |
| urf | عرف | custom |
| ta'zir | تعزير | penalties set by the authorities |

*Mahmiyya* comes from the same root as *hima*, but it is not the same word. Please record them separately. We do not yet know whether *hima* itself appears in any current law, so a `none` is just as useful as a find.

Words in a law's preamble or explanatory note count too. Please write `preamble` or `explanatory note` instead of an article number.

## Points we already found

- **Oman:** Royal Decree 53/1981, the old fishing law, was **repealed** by Royal Decree 20/2019, the Living Aquatic Resources Law.
- **Bahrain:** the fishing law, Decree-Law 20/2002, was amended in 2012. It was amended again by Law 14/2025, which raised the fines.
- **Bahrain:** the environment law of 1996 was replaced by Law 7/2022.
- **Qatar:** the fishing law, Law 4/1983, is still in force. It was amended in 1995, 2003 and 2010.
- **Saudi Arabia and Kuwait:** no rows have been checked yet. The official sites were slow or did not open from our side, so local access would help most here.

## How to send changes back

You can do either of the following:

- Edit the file on GitHub, using the pencil icon on the file page.
- Download the file, edit it in Excel, and email it back to us. We will merge it.
