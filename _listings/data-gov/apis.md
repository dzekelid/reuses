---
name: Data.Gov
x-slug: data-gov
description: data.gov is a U.S. government website launched in late May 2009 by the
  then Federal Chief Information Officer (CIO) of the United States, Vivek Kundra.
  According to its website, The purpose of data.gov is to increase public access to
  high value, machine readable datasets generated by the Executive Branch of the Federal
  Government. The site seeks to become a repository for all the information the government
  collects. The site would publish to the public any data that is not private or restricted
  for national security reasons.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Reuses
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/apis.md
specificationVersion: "0.14"
apis:
- name: Data.gov API - Get Me Org Reuses
  x-api-slug: meorg-reuses-get
  description: List all reuses related to me and my organizations
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/meorg-reuses-get-openapi.md
- name: Data.gov API - Get Me Reuses
  x-api-slug: mereuses-get
  description: List all my reuses (including private ones)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/mereuses-get-openapi.md
- name: Data.gov API - Get Organizations Org Reuses
  x-api-slug: organizationsorgreuses-get
  description: List organization reuses (including private ones when member)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/organizationsorgreuses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/organizationsorgreuses-get-openapi.md
- name: Data.gov API - Get Reuses
  x-api-slug: reuses-get
  description: Get Reuses
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reuses-get-openapi.md
- name: Data.gov API - Add Reuses
  x-api-slug: reuses-post
  description: Create a new object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reuses-post-openapi.md
- name: Data.gov API - Get Reuses Badges
  x-api-slug: reusesbadges-get
  description: List all available reuse badges and their labels
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesbadges-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesbadges-get-openapi.md
- name: Data.gov API - Get Reuses Suggest
  x-api-slug: reusessuggest-get
  description: Suggest reuses
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusessuggest-get-openapi.md
- name: Data.gov API - Get Reuses Types
  x-api-slug: reusestypes-get
  description: List all reuse types
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusestypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusestypes-get-openapi.md
- name: Data.gov API - Delete Reuses  Followers
  x-api-slug: reusesidfollowers-delete
  description: Unfollow an object given its ID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesidfollowers-delete-openapi.md
- name: Data.gov API - Get Reuses  Followers
  x-api-slug: reusesidfollowers-get
  description: List all followers for a given object
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesidfollowers-get-openapi.md
- name: Data.gov API - Add Reuses  Followers
  x-api-slug: reusesidfollowers-post
  description: Follow an object given its ID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesidfollowers-post-openapi.md
- name: Data.gov API - Delete Reuses Reuse
  x-api-slug: reusesreuse-delete
  description: Delete a given reuse
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesreuse-delete-openapi.md
- name: Data.gov API - Get Reuses Reuse
  x-api-slug: reusesreuse-get
  description: Fetch a given reuse
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesreuse-get-openapi.md
- name: Data.gov API - Put Reuses Reuse
  x-api-slug: reusesreuse-put
  description: Update a given reuse
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesreuse-put-openapi.md
- name: Data.gov API - Add Reuses Reuse Badges
  x-api-slug: reusesreusebadges-post
  description: Create a new badge for a given reuse
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesreusebadges-post-openapi.md
- name: Data.gov API - Delete Reuses Reuse Badges Badge Kind
  x-api-slug: reusesreusebadgesbadge-kind-delete
  description: Delete a badge for a given reuse
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesreusebadgesbadge-kind-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesreusebadgesbadge-kind-delete-openapi.md
- name: Data.gov API - Add Reuses Reuse Datasets
  x-api-slug: reusesreusedatasets-post
  description: Add a dataset to a given reuse
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesreusedatasets-post-openapi.md
- name: Data.gov API - Delete Reuses Reuse Featured
  x-api-slug: reusesreusefeatured-delete
  description: Unmark a reuse as featured
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesreusefeatured-delete-openapi.md
- name: Data.gov API - Add Reuses Reuse Featured
  x-api-slug: reusesreusefeatured-post
  description: Mark a reuse as featured
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesreusefeatured-post-openapi.md
- name: Data.gov API - Add Reuses Reuse Image
  x-api-slug: reusesreuseimage-post
  description: Upload a new reuse image
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/reusesreuseimage-post-openapi.md
- name: Data.gov API - Get Site Home Reuses
  x-api-slug: sitehomereuses-get
  description: List homepage featured reuses
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/sitehomereuses-get-openapi.md
- name: Data.gov API - Put Site Home Reuses
  x-api-slug: sitehomereuses-put
  description: Set the homepage reuses editorial selection
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/data-gov-logo.png
  humanURL: http://data.gov/
  baseURL: https://catalog.data.gov//api/3/
  tags: Federal Government, Federal Government, Federal Government   GSA, Stack Network,
    Data Provider, API Provider, Profiles, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/reuses/master/_listings/data-gov/sitehomereuses-put-openapi.md
x-common:
- type: x-api-gallery
  url: http://danske.bank.api.gallery.streamdata.io
- type: x-api-stack
  url: http://data.gov.stack.network
- type: x-blog
  url: https://www.data.gov/meta/
- type: x-blog-rss
  url: https://www.data.gov/feed/
- type: x-developer
  url: http://developer.data.gov/
- type: x-signup
  url: https://api.data.gov/signup/
- type: x-twitter
  url: https://twitter.com/usdatagov
- type: x-website
  url: http://data.gov/
- type: x-wikipedia
  url: http://en.wikipedia.org/wiki/Data.gov
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---