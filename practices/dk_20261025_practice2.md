# Question
A virtual memory management system in an operating system uses First-In-First-Out (FIFO) cache.

When a requested memory page is not in the cache and the cache is full, the page that has been in the cache for the longest duration is removed to make room forthe requested page. If the cache is not full, then the requested page can simplybe added to the cache. A given page should occur once in the cache at most.

Given the maximum size of the cache and an array of page requests, calculate the number of cache misses. A cache miss occurs when a page is requested but is not found in the cache. Initially, the cacheis empty.

# Input
The first line of the input consists of an positive integer - page_requests_size, representing the total number of pages(N).

The second line contains N space-separated positive integers - page_requests[0], page_requests[1],.. page_requests[N-1], representing the page requests for N pages.

The last line consists of an integer - max_cache_size, representing the size ofthe cache.

# Output
Print an integer representing the numberof cache misses.

# Note
Assume that the array page_requests contains pages numbered in the range 1-50. A page at index i in page_requests is requested before a page at index i+1.

# Example
Input:
6
1 2 1 3 1 2
2

Output:
5

Explanation:
Cache state as requests come in ordered longest-time-in-cache to shortest-time-in-cache:
1 *
1 2 *
1 2
2 3 *
3 1 *
1 2 *

Asterisk(*) represents a cache miss. So the total number of cache misses is 5.
