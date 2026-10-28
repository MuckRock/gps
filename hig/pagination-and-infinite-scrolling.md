# Pagination and infinite scrolling

Most of our API endpoints use cursor-based pagination, rather than the less-efficient offset/limit approach that Django defaults to. As a consequence, it’s easy for us to say “get the next page of results” but hard to say “get page X.”

Given this tradeoff, we usually prefer an infinite scroll approach to pagination. A user loads the first page of results immediately and then sees more upon scrolling down. We use intersection observers to track scroll depth and load the next page when the user reaches the bottom.

If something goes wrong in that flow, we show a “Load next” button, so the user can still get to the next set of results, or see an error message if the request fails.

There is a downside to this: If the user scrolls several pages down and then reloads the page, we can only show the first page of results. We don’t know how many pages were loaded, and cursors only point to the next set of results, not any specific result set. (This would be true even if we tried to fake numbered pages.)
