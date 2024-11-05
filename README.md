
# Basel GitHub Users Data Analysis

- **Scraped Data Collection**: Data was collected from the GitHub API by filtering users in Basel with more than 10 followers and gathering information on their public repositories.
- **Interesting Finding**: Over 40% of Basel users have less than 5 repositories, but most work in popular languages like Python and JavaScript.
- **Recommendation**: Basel developers could increase visibility by engaging more in open-source contributions, especially in trending languages like Rust and Go.

## Project Overview

This repository contains data about GitHub users in Basel with more than 10 followers, including their public repositories. The goal is to analyze user activity, language preference, and engagement in the Basel GitHub community.

### Files

1. **`users.csv`** - Contains information on each user from Basel with over 10 followers.
2. **`repositories.csv`** - Contains information on each user’s public repositories, up to 500 repositories per user.
3. **Optional**: Analysis script in Python (or chosen language), if provided.

### Fields

- **users.csv**: `login`, `name`, `company`, `location`, `email`, `hireable`, `bio`, `public_repos`, `followers`, `following`, `created_at`
- **repositories.csv**: `login`, `full_name`, `created_at`, `stargazers_count`, `watchers_count`, `language`, `has_projects`, `has_wiki`, `license_name`

## Data Collection Process

The data was collected using the GitHub API. Here’s a quick overview of the process:

1. **User Filtering**: Queried for users in Basel with more than 10 followers.
2. **Data Transformation**: For each user, cleaned and normalized fields such as `company` by:
    - Removing whitespace,
    - Stripping any leading "@" symbol,
    - Converting names to uppercase.
3. **Repository Collection**: For each user, retrieved up to 500 of their most recent repositories, storing relevant fields such as `stargazers_count`, `watchers_count`, and `language`.

## Analysis Summary

After examining the data, we found:

- **Language Preferences**: Python and JavaScript are the most commonly used languages in Basel.
- **Engagement Levels**: The average follower count is around 20, with most users having small follower and following counts.
- **Repository Activity**: A large number of users have fewer than 5 public repositories.

## Recommendations for Basel Developers

- **Expand Repository Activity**: To increase visibility, developers could contribute to more repositories and engage in collaborative projects.
- **Explore New Languages**: Engagement in fast-growing languages like Rust and Go could set Basel developers apart.
- **Build Stronger Networks**: Engaging with peers on GitHub could foster a more active local community.

## How to Use

1. Clone the repository.
2. Use the `users.csv` and `repositories.csv` files for data analysis or integration into a larger project.

