---
title: Ruby on Rails Pt. 1
date: 2019-05-20 14:41:51
tags:
---
During my internship this summer at OpenStax, I had to learn and work with Ruby on Rails. Aside from two 2-hour long crash courses given by my supervisor at the beginning of the summer, I was pretty much on my own figuring out how to navigate the endless directories and files in a rails project, all with distinct roles and interactions.

## Confusion
In a single rails project, there are several directories (app, bin, config, db, lib, log, public, spec...) that seem to go on and on and upon first glance, I had no idea what any of them did. After the crash course, I learned that the `spec` folder contains specs, which are supposedly 'human-readable' test files - I would have initially argued the 'human-readable' part. 

However, as I practiced what we had gone over in the crash course, I started to see how a seemingly weirdly-worded body of code such as:
	`context "when sent a valid input" do`
		`it "status is 200 (success)`
			`expect(status).to eq(200)`
would print the almost-English statement, "when sent a valid input, status is 200" message upon running the test to check the status, and how this would become especially helpful for reading tests when running many at once.

The spec file I was assigned to write required me to deal with mock objects, and understand the interactions between routes, controllers (what is a controller???), and other classes, none of which I had the faintest idea about, leading to much panic and confusion piled on top of nerves from starting my first software internship and an overwhelming fear of disappointing my supervisor.
{% asset_img confused_coder.png Confused Coder %}

It ended up taking me several workdays to painfully write out just a few coherent specs in a spec file, but after that I began to get the hang of it. (or so I thought)

To be continued...


