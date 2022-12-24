# 100 years of the A-Matrix


In the year 1922, Sewall Wright first documented the idea of tracing paths to establish the [relationships](https://www.jstor.org/stable/2456273#metadata_info_tab_contents) among animals. Though he was not working in the field of agriculture, his discovery laid the **path** (pun intended) toward revolutionizing the breeding and agriculture sector. Followed by Wright, scientists like Thompson, Henderson, Quaas, Meuwissen, Luo, Van Vleck, Mistzal, and many others extended his idea and derived the A-matrix or additive genetic relationship matrix or Numerator Relationship Matrix (NRM), Inverse of A-matrix (more realistic), and finally the Genomic Relationship Matrix (exploiting the Mendelian sampling term). These matrices are used to quantify the relationship between individuals in a population based on their genetic makeup. This is one of the four main pillars in estimating breeding values of animals (BLUP). Ways of computing the A/G-matrix more efficiently is still an active field of research in animal breeding.

The pictures below provide a glimpse of the after-effect of Wright's work over the past 100 years.


![No alt text provided for this image](https://media.licdn.com/dms/image/D5612AQFn4MhzGbWEZQ/article-inline_image-shrink_1500_2232/0/1671735047482?e=1677110400&v=beta&t=tP2NjrgOTT8NFtYcMigC-Vw_eUiJLZi3wRmJQYEVeXo)

<p style="text-align: center;">Credits: Julius Van Der Werf

![No alt text provided for this image](https://media.licdn.com/dms/image/D5612AQF-EoLZdnjbzQ/article-inline_image-shrink_1500_2232/0/1671735087011?e=1677110400&v=beta&t=PNT4b9ycE7YOF85_dq0bvtBhVXB6UJEBgKWMT8ly6gg)

<p style="text-align: center;">Credits: Harold(2014)

Today, R and Julia scripts can be written for calculating the A-matrix.

```
julia> show(stdout, "text/plain",ped
8×3 Matrix{Int64}:
 1  0  0
 2  0  0
 3  0  0
 4  1  0
 5  3  2
 6  1  2
 7  4  5
 8  3  6
julia> show(stdout, "text/plain", A)
8×8 Matrix{Float64}:
 1.0   0.0   0.0   0.5    0.0    0.5   0.25  0.25
 0.0   1.0   0.0   0.0    0.5    0.5   0.25  0.25
 0.0   0.0   1.0   0.0    0.5    0.0   0.25  0.5
 0.5   0.0   0.0   1.0    0.0    0.25  0.5   0.125
 0.0   0.5   0.5   0.0    1.0    0.25  0.5   0.375
 0.5   0.5   0.0   0.25   0.25   1.0   0.25  0.5
 0.25  0.25  0.25  0.5    0.5    0.25  1.0   0.25
 0.25  0.25  0.5   0.125  0.375  0.5   0.25  1.0

Credits: Austin Putz, Gota Morota
```

GRM is the latest tool in GEBV estimation.

![No alt text provided for this image](https://media.licdn.com/dms/image/D5612AQEZUlr-PmH6Gg/article-inline_image-shrink_1500_2232/0/1671735216502?e=1677110400&v=beta&t=tj3vTxXfXbS9Lb_1pfWdAtuP2_b5g5OScvGaqg-mE7k)

<p style="text-align: center;">Credits: Jiang(2019)

As we can see, the ripple effect of Wright's work is very large and still going strong. I know, I have missed many points regarding the topic. Do share your thoughts on the current state of research in this area and what the future trends may be.
