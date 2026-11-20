+++
title = "TNAU Agriculture Events"
description = "Collects TNAU AgriTech Portal's Press Notes that are published as PDF files, parses them into structure events data using LLM, translates the events data in Tamil and renders in an intuitive UI."
date = 2026-01-08

[extra]
local_image = "projects/tnau-agri-events-screenshot.jpg"
invertible_image = false

[taxonomies]
tags = ["web app", "agriculture", "supabase", "reactjs", "gen ai"]
+++

{{< dimmable_image src="tnau-agri-events-screenshot.jpg" alt="A screenshot of T N A U Agri Events web app showing 0 ongoing events and first two of the 20 past events. The web app's content is in Tamil language. Above the results a search field and a set of filter options named 'All Events', 'Training', 'Announcements', etc. are shown with 'All Events' button selected." />}}

[**TNAU Agriculture Events**](https://agri-events-ui.vercel.app/) collects [TNAU AgriTech Portal's Press Notes](https://agritech.tnau.ac.in/tnaupressnotes/pnindex2026.html) that are published as PDF files, parses them into structure events data using LLM, translates the events data in Tamil and renders in an intuitive UI.

It uses  [ReactJS](https://reactjs.org/), [Tailwind CSS](https://tailwindcss.com/), [shadcn/ui](https://ui.shadcn.com/docs/components), and [react-i18next](https://react.i18next.com/) in **frontend**, [Supabase](https://supabase.io/) (Postgres data store), [pymupdf](https://pymupdf.readthedocs.io/en/latest/) (for PDF parsing), [dspy](https://dspy.ai/) (declarative framework for LLM calls), [Gemini](https://gemini.google/about/) (for events extraction from parsed PDF texts), [sarvamai](https://www.sarvam.ai/text) (for translation of events data from English to Tamil), [Google Cloud Run Jobs](https://cloud.google.com/run?hl=en#batch-data-processing) (for hosting scheduled background jobs) in **backend**, and [Vercel](https://vercel.com/) for frontend hosting.
