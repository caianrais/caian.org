---
layout: default
title: Homepage
---

# Caian R. Ertl

This website is mainteined as my personal online cave, to make public some of
what I am, what I like and do. If you're the NSA or any data mining company,
this is probably the best you have since I'm not on social media.

## whois caian.org

A 21 years old programmer living in [São Paulo, Brazil][home] who works as an
infrastructure developer (DevOps) for [Mandic][work] and is an undergraduate
student at the [Anhembi Morumbi][uni] university.

I deeply value privacy, anonimity, freedom of information exchange and
minimalism (both functionally and aesthetically, though i'm not quite sure
where the line should be drawn).

- [GitHub](https://github.com/caiertl)
- [LinkedIn](https://linkedin.com/in/caiertl)
- [Curriculum Vitae](assets/pdf/cv_en.pdf) (pdf) / ([pt_BR](assets/pdf/cv_pt.pdf))

## Blog

[All posts](/blog.html)
{% for post in site.categories.tech limit: 3 %}
- `{{ post.date | date: "%Y-%m-%d" }}` - [{{ post.title }}]({{ post.url }}) {% endfor %}

## Projects

[All projects](/projects.html)

- [tmul][tmul], a tiny implementation of a Lisp-like language
- [dora][dora], a cloud-ready DNS query microservice
- [coin][coin], a CLI tool to currency conversion
- [tpsp][tpsp], a CLI tool to get São Paulo's [train][cptm] and [metro][metro] lines statuses
- [vault-auth-google][vag], a [Vault][vault] plugin that authenticates with Google


{% comment %}
    "about-me" references.
{% endcomment %}

[home]: https://bit.ly/2hx2Tdv
[work]: https://mandic.com.br
[uni]: https://portal.anhembi.br

{% comment %}
    Hyperlinks of the projects
{% endcomment %}

[tmul]:  https://github.com/caian-org/tmul
[dora]:  https://github.com/caian-org/dora
[coin]:  https://github.com/caian-org/coin
[tpsp]:  https://github.com/caian-org/tpsp
[vag]:   https://github.com/erozario/vault-auth-google

{% comment %}
    References to the products/services
{% endcomment %}

[vault]: https://vaultproject.io
[drone]: https://drone.io
[cptm]:  https://www.cptm.sp.gov.br
[metro]: http://www.metro.sp.gov.br