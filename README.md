# Jarvis English Course

This public repository contains the English course materials and assessment pages.

## Files
- `index.html` — Student English test (20 MCQs + writing task).
- `test.html` — Alternate copy of the student test.
- `teacher.html` — Teacher dashboard with Supabase Auth sign-in.
- `lecture1.html` — First lesson, speaking activities, 100 B2 words and 50 expressions.

## Supabase connection
The student test and teacher dashboard connect to the dedicated English Test Supabase project:
- Project URL: `https://ruliophlnvsexzjekdbs.supabase.co`
- Uses a publishable client key only. No service-role or secret key is included.

Student submissions are stored in `english_test_attempts`. Teacher access is controlled by Supabase Auth and the RLS policies for the approved teacher account. Keep those policies enabled; never add public SELECT access or a service-role key to these pages.

## Important
This repository is public. Do not add passwords, secret keys, private student information, or service-role credentials. The teacher dashboard requires an authorized teacher login; publishing its source does not make student records public.
