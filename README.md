# Email Draft Builder

A browser-based utility for turning copied emails or business requests into reusable email drafts. Paste text from any source, review the information detected by simple rules, customize the subject and body templates, select local attachments, and download an `.eml` file.

## Features

- Accepts copied text from email clients, collaboration tools, documents, or other sources. It does not depend on one request form.
- Tries to identify common fields such as a subject, name, email address, date, deadline, URL, quantity, and details. Results are editable because source formats vary.
- Supports reusable subject and body templates with placeholders.
- Adds files selected from the user's device to the downloaded EML draft.
- Runs in the browser, requires no mail API key, and never sends messages automatically.

## Run

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Copy an email or request into **원문 메일 또는 요청 내용**. The source may be from any platform.
4. Select **정보 추출**, review and correct the fields, then enter the recipient and any response text.
5. Edit the subject or body template if needed, and select any files to attach.
6. Download the EML file and open it with a compatible mail client. Review the draft and send it yourself.

## Template placeholders

Use these placeholders in the subject and body templates:

`{{source_subject}}`, `{{source_text}}`, `{{name}}`, `{{email}}`, `{{date}}`, `{{deadline}}`, `{{url}}`, `{{quantity}}`, `{{details}}`, and `{{response}}`.

Information extraction is best-effort and based on common labels and patterns; always review the generated draft. The tool does not automatically read a mailbox or fetch its attachments. Copy source text and download/select any attachments yourself.

## Privacy

- The page does not send pasted text, recipient addresses, or selected attachments to a server.
- Email addresses and draft content are not saved by the tool.
- The downloaded `.eml` contains the recipients, subject, body, and selected attachments. Treat it as an email draft containing potentially sensitive information.
- Do not add real emails, customer data, or private attachments to this public repository.
