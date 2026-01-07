# Supernova writing guidelines

As the number of designers and engineers working on and accessing the documentation has increased, we need to define guidelines to ensure our writing style is consistent across our entire documentation site, to avoid confusion and misalignment.

<aside>
⚠️ These guidelines have been imported from Back Market’s documentation guidelines, with slight updates to fit Accor’s contexts.

</aside>

To make the best use of these guidelines, pair them with the free [Grammarly](https://app.grammarly.com/) plugin and Socrates ([accor-gpt-assistant](https://accor-gpt.accor.net/?models=d0af56f4-725d-43c8-b82c-be64a50748c9)) when writing documentation. The assistant will help you to adapt any guidelines to the desired format/tone of voice (detailed below).

[Ongoing discussion](https://www.notion.so/Ongoing-discussion-12ebadc8975180f9a91def22602d4f97?pvs=21)

# General writing style

## Write for everyone

The design system documentation is open to everyone at Accor, not only to the Welcome team. Follow these points to ensure that everyone can easily understand everything.

Use standard English expressions rather than idioms to make sure everyone can understand. Even though English is the company language, not everyone is a native speaker.

Use simple and clear language. Be specific, provide context, use short phrases, and use graphics to convey complex information. If you need to use technical terms or acronyms, define them briefly to ensure everyone can understand. Avoid unnecessary modifiers, jargon, and vague language.

## Use active voice

Active voice, clarifying the performer of an action, makes sentences easier to understand. On the other hand, passive voice identifies the recipient of the action as the subject of the verb, making a text less engaging and more complicated.

<aside>
✅ Create a component.

</aside>

<aside>
🚫 A component is created.

</aside>

Only use passive voice if using active voice makes it sound like you are blaming the users.

<aside>
✅ If components don’t appear up-to-date, the library might not have been uploaded.

</aside>

<aside>
🚫 If components don’t appear up-to-date, you probably didn’t upload the library.

</aside>

## Write positively

Write in positive language rather than in negative language. Positive language improves readability, keeps the tone friendly, and the sentences short.

<aside>
✅ Follow the Contribution Guidelines to contribute to Welcome.

</aside>

<aside>
🚫 You can’t contribute to Welcome if you don’t follow the Contribution Guidelines.

## Use the present tense.

Users read documentation to perform tasks or gather information, and for them, these activities take place in their present, so the present tense is appropriate in most cases.

Use the future or past tense only when you need to emphasize that something has occurred in the past or will occur later.

<aside>
✅ We used to use Garamond in the past, so you might still find it in use in older files.

</aside>

## Addressing others

Write in the second person to address users directly. This will make the documentation more friendly and engaging.

<aside>
✅ To add a new paragraph, click on the “+” icon on the left.

</aside>

<aside>
🚫 Adding a new paragraph requires clicking on the “+” icon on the left.

</aside>

</aside>

## Writing about others

Accor is an international, multicultural, and diverse company. Our documentation language should take this into account. Make sure your documentation is free from words, phrases, or tones that may sound prejudiced, stereotyped, or discriminatory towards particular people or groups.

Write in first person plural when talking about Accor and the Welcome team. If relevant, you can specify a person, for example as a point of contact.

<aside>
✅ At Welcome, we believe every question has an answer.

</aside>

<aside>
🚫 At Welcome, I believe every question has an answer.

</aside>

Write in gender neutral language and use “they” as a singular pronoun when referring to an unspecified person, and use neutral terms instead of gendered ones to avoid making a specific gender invisible.

Use non-ableist language and make sure you’re not using phrases that are biased and that victimize people with disabilities.

<aside>
✅ Users who have dyslexia.

</aside>

<aside>
🚫 Users who suffer from dyslexia.

</aside>

Use culturally sensitive language. Be mindful of the different cultures the users are part of and their different ethnicities. Don’t use expressions that have religious, cultural, or racial connotations or that are insensitive in these regards.

<aside>
✅ A beige background.

</aside>

<aside>
🚫 A nude background.

</aside>

## Be consistent

Consistency is essential in establishing a shared vocabulary. Using these guidelines as your reference when writing documentation will reduce the risk of confusion and the need for further clarification for the users.

# UI terminology

## Design System (DS)

Always spell Design System in title case when talking about a specific one (namely, Welcome). When writing about design systems in general, use sentence case and the plural (or adjective) form.

<aside>
✅ Our Design System, Welcome, is now open to the public.

</aside>

<aside>
✅ Ask a Design System Manager for support.

</aside>

<aside>
✅ For design system-related questions, head over to Teams.

</aside>

<aside>
✅ Design systems are like toolboxes.

</aside>

## Users

There are two types of users, internal users and end users. Accor employees, contractors, or external agencies accessing our documentation are the internal users, while our platform users are the end users. Depending on the context, you might have to specify the type of users for the sake of clarity.

Always use the plural form when talking about users of any type – this will prevent you from having to specify a gender.

<aside>
✅ Our internal users want to ensure the UI is accessible to our end users.

</aside>

<aside>
🚫 Our users want to ensure the UI is accessible to them.

</aside>

## Components

Consider specific component names as proper nouns. Use the singular form when writing about them (including variants and states) and use title case to make them easier to spot: this also applies to local components (e.g., Booking Engine) or we don’t have yet (e.g. Form).

Components containing multiple elements like Tabs and Breadcrumbs should end with an “s”, but still referred as singular nouns.

When mentioning components, write as if they were formal concepts (or people): “Date Picker is used when…” / “Use Breadcrumbs to…”, without articles.

Use the plural form and sentence case when talking about components in general. When describing a group of certain components, use plural, or the phrase “Component item”. Avoid prefixing components with “The”.

For an extra highlight, it can be useful to link the component page to the label.

<aside>
✅ Card has been updated to have fewer variants.

</aside>

<aside>
✅ Use Tabs to organize similar content across screens in a single area.

</aside>

<aside>
🚫 The Breadcrumbs can help navigate the site’s structure.

</aside>

<aside>
✅ We use 3 types of buttons in our UI.

</aside>

<aside>
✅ Accordions can be grouped in sections of up to 8 items.

</aside>

<aside>
✅ Button Primary in the Focus state has sufficient contrast for accessibility.

</aside>

## Variants and properties

Although variant and property names are written in lowercase in Figma, write them in title case in the Supernova documentation. This helps them stand out as unique objects.

For values, use the code format, except when they are used in titles or first words of a sentence.

<aside>
✅ Lastly, Emphasis controls the visual weight of the component, and can be either `default` or `highlight`.

</aside>

<aside>
🚫 Use the `primary` Button once per page *(as a title)*

</aside>

## Breakpoints

In the spirit of being mobile-first, Breakpoints should be documented starting with mobile and going up. Mobile is the default view (as it is in Figma, the default variant, when applicable).

## Token names

Write token names in lower case and use the “Code” button from the Supernova editor toolbar. The word “Token” itself should be written in title case.

<aside>
✅ Color Tokens are available as JSON in the Single Source of Truth (SST).

</aside>

<aside>
✅ The background uses the `surface-container-min` token.

</aside>

## Color codes

In Supernova, use the “Code” editor button for color codes.

<aside>
✅ The base color is `#FFFFFF`.

</aside>

## Keyboard keys

Write keyboard keys in uppercase and use the Supernova “Code” editor button to highlight them.

<aside>
✅ Using `TAB`, users can navigate through the Card’s child elements.

</aside>

<aside>
🚫 Use the tab to show focus rings.

</aside>

# Grammar and standards

In alphabetical order

## Abbreviations, acronyms, internal names

If there’s the possibility the users won’t recognize an abbreviation, an acronym, or an internal name, spell it out the first time you mention it on a page. Then you can use the shortened version for all other references. However, if the abbreviation or acronym is well known, like HTML or CSS, you can use it straight away without the need to spell it out.

<aside>
✅ The DAM (Digital Assets Manager) is a repository for assets. Upload your pictures to the DAM via this process.

</aside>

Don’t use apostrophes for plural abbreviations.

<aside>
✅ PNGs.

</aside>

<aside>
🚫 PNG’s.

</aside>

Don’t use periods in acronyms and abbreviations.

<aside>
✅ The USA.

</aside>

<aside>
🚫 The U.S.A.

</aside>

## I.e. vs e.g.

E.g. (Latin: *exempli gratia* → literally “for the sake of example”) means “for example”, while i.e. (Latin: *id est* → literally “that is”) means “in other words”. E.g. provides one or more examples on a topic. I.e. provides more precise information narrowing down the options.

<aside>
✅ Welcome offers several Input components, e.g. Date, Currency, etc.

</aside>

<aside>
✅ This component is responsive, i.e. it can change according to screen sizes.

</aside>

## Capitalization

Use sentence case in all titles, headings, labels, and menu items.

<aside>
✅ Get started

</aside>

<aside>
🚫 Get Started

</aside>

Use [title case](https://en.wikipedia.org/wiki/Title_case) for component, foundations, patterns, assets, and page (in our products) names. This includes talking about a component (e.g talking about Accordion) but also when talking about the conceptual group in the DS.

When talking about components (and other elements) in general within a sentence, use sentence case.

<aside>
✅ Button Primary, Search Results

</aside>

<aside>
🚫 Button icon

</aside>

<aside>
✅ Grid & Breakpoints

</aside>

<aside>
✅ Dark mode

</aside>

<aside>
✅ Design System glossary

</aside>

<aside>
✅ Learn more about Components.

</aside>

<aside>
✅ This newly added element is a pattern.

</aside>

<aside>
🚫 This Component is only available on AEM.

</aside>

<aside>
✅ The padding is the same in both mobile and tablet Breakpoints.

</aside>

In case of brands or product names, follow their own capitalization rules even if they differ from ours.

<aside>
✅ GitLab

</aside>

<aside>
🚫 Gitlab

</aside>

Use lower case for URLs, email addresses, file names, and Slack channels (not Teams channels).

<aside>
✅ #ds-review on Slack

</aside>

Don’t use all caps in general documentation. Use bold or a callout to emphasize text instead. However, use it in technical documentation, when it’s the standard for programming languages.

## Code

Use the “Code” button from the Supernova editor toolbar when writing color codes and token names. From the same toolbar, use the “Code” prompt (”/code”) to add code snippets.

## Contractions

Use contractions to keep a friendly and conversational tone throughout our documentation. Don’t use contractions if you want to add emphasis to a sentence, for example, in warnings.

<aside>
✅ This page is outdated, do not use it as a reference.

</aside>

## Dates

For simplicity’s sake, given the majority demographic in the design team, use the French standard for dates, DD/MM/YYYY, with a slash (”/”) between numbers.

<aside>
✅ 24/08/2024

</aside>

<aside>
🚫 2024-08-24

</aside>

## Emojis

Emojis can be helpful as icons in the text editor. However, use them only if they help clarify the information provided, not as conversational prompts or for purely illustrative purposes in Supernova. Overusing them will make the page look cluttered.

<aside>
✅ ⚠️ Caution

</aside>

<aside>
🚫 Card has three variants. 💪🏻

</aside>

<aside>
🚫 The 🎨 Color Tokens are split into two families.

</aside>

<aside>
🚫 Welcome 👋🏻

</aside>

## Emphasis

Use bold to draw attention to keywords or short statements. Use a callout to highlight a slightly longer text, such as a note (use blue) or a warning (use yellow). Use italics for citations and other languages only.

## Lists

Use lists to make a sequence of items easier to scan and follow. Lists can be of two types, bulleted or numbered.

Use bulleted lists when the order of the items isn’t relevant, and use numbered lists when the order matters.

Use a [colon](https://en.wikipedia.org/wiki/Colon_(punctuation)) to introduce bulleted and numbered lists. Phrase each list item in a parallel way and capitalize the first word in each item. If items are complete sentences, end each of them with a period.

<aside>
✅ A Button can act as a call to action, for example:
– To submit a Form.
– To open a Modal.
– To anchor links within the same page.

</aside>

<aside>
🚫 A Button can act as a call to action, for example.

1. Submit a Form
2. Open a Modal
3. anchor links within the same page
</aside>

## Numbers

In English, decimals are written with a point and thousands with a comma.

<aside>
✅ 5,000,000 (five million), 1.5 (one point five).

</aside>

<aside>
🚫 5 000 000 or 5.000.000 (five million), 1,5 (one point five).

</aside>

## Punctuation

### Ampersand

Don’t use “&” instead of “and” unless it’s part of a brand, a product, or a section name.

<aside>
✅ Copy and paste

</aside>

<aside>
✅ Grid & Breakpoints

</aside>

<aside>
🚫 Save & upload

</aside>

### Colon

Use a colon to introduce a list or a series of steps, or to start an explanation. Don't use colons at the end of titles or headings. Warning: In English, colons aren’t followed by a space.

<aside>
✅ For example, `surface-container-min` can be paired with `on-surface-hi`.

</aside>

<aside>
🚫 Keep in mind the following: Components are built on Foundations.

</aside>

### Dashes

Use hyphens ( - ) with no spaces around to write ranges. Use em dashes ( — ) with spaces around to indicate an aside or an abrupt change in a sentence. Press option-shift-hyphen to make an em dash on a Mac.

<aside>
✅ Choose a value (1-100) and press `ENTER`.

</aside>

<aside>
✅ Use em dashes sparingly — the sentences should be as simple as possible.

</aside>

### Dashes

Use exclamation marks to convey more energy and positivity in a sentence. Use them with moderation, otherwise they will lose their meaning.

### Serial comma

Use the serial comma (Oxford comma) before the “and” and “or” conjunctions that connect items in a list.

<aside>
✅ We use sentence case in titles, headings, and menu items.

</aside>

<aside>
🚫 We use sentence case in titles, headings, and menu items.

</aside>

### Space

Leave a single space between sentences and follow the standard English spacing rules. Specifically, don’t use a space before punctuation marks.

### Quotation marks

Use the standard US English quotation marks (“ “). Use single quotation marks (' ') to quote inside a quote. Periods go inside quotation marks. Don’t use guillemets (« ») or inverted commas („ ”).

## Spelling

Use the US spelling in our documentation. The company policy doesn’t set a standard in internal facing documents, but in our case it’s a matter of consistency across the entire documentation site that has several contributors.

When in doubt, run your text through a spelling or grammar checking tool. The following rules should cover most cases, though.

British English words ending in “tre” usually end in “ter” in US English.

<aside>
✅ Center

</aside>

<aside>
🚫 Centre

</aside>

British English words ending in “our” usually end in “or” in US English.

<aside>
✅ Color

</aside>

<aside>
🚫 Colour

</aside>

British English verbs ending in “ise” and “yse” usually end in “ize” and “yze” in US English.

<aside>
✅ Analyze, organize

</aside>

<aside>
🚫 Analyse, organise

</aside>

In US English, the “l” is not doubled in verbs ending in a vowel + “l”.

<aside>
✅ Traveling

</aside>

<aside>
🚫 Travelling

</aside>

## Titles

Use sentence case in all documentation titles and headings. Don't use bold, italics, or standard punctuation like periods and colons. You can use question marks if relevant.

## Letters or

Chiffres à la place des lettres