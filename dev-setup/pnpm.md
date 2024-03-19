# PNPM

## Saving disk space

<p align="center">
<img src="data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjwhRE9DVFlQRSBzdmcgUFVCTElDICItLy9XM0MvL0RURCBTVkcgMS4xLy9FTiIgImh0dHA6Ly93d3cudzMub3JnL0dyYXBoaWNzL1NWRy8xLjEvRFREL3N2ZzExLmR0ZCI+CjxzdmcgeG1sbnM6eGw9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHhtbG5zOmRjPSJodHRwOi8vcHVybC5vcmcvZGMvZWxlbWVudHMvMS4xLyIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjExMC41IDEyMSA2NTkuMjk0NCAyNzIuODM1OTQiIHdpZHRoPSI2NTkuMjk0NCIgaGVpZ2h0PSIyNzIuODM1OTQiPgogIDxkZWZzPgogICAgPG1hcmtlciBvcmllbnQ9ImF1dG8iIG92ZXJmbG93PSJ2aXNpYmxlIiBtYXJrZXJVbml0cz0ic3Ryb2tlV2lkdGgiIGlkPSJGaWxsZWRBcnJvd19NYXJrZXIiIHN0cm9rZS1saW5lam9pbj0ibWl0ZXIiIHN0cm9rZS1taXRlcmxpbWl0PSIxMCIgdmlld0JveD0iLTEgLTQgMTAgOCIgbWFya2VyV2lkdGg9IjEwIiBtYXJrZXJIZWlnaHQ9IjgiIGNvbG9yPSIjN2Y4MDgwIj4KICAgICAgPGc+CiAgICAgICAgPHBhdGggZD0iTSA4IDAgTCAwIC0zIEwgMCAzIFoiIGZpbGw9ImN1cnJlbnRDb2xvciIgc3Ryb2tlPSJjdXJyZW50Q29sb3IiIHN0cm9rZS13aWR0aD0iMSIvPgogICAgICA8L2c+CiAgICA8L21hcmtlcj4KICA8L2RlZnM+CiAgPGcgaWQ9IkNhbnZhc18xIiBzdHJva2UtZGFzaGFycmF5PSJub25lIiBmaWxsPSJub25lIiBzdHJva2Utb3BhY2l0eT0iMSIgZmlsbC1vcGFjaXR5PSIxIiBzdHJva2U9Im5vbmUiPgogICAgPHRpdGxlPkNhbnZhcyAxPC90aXRsZT4KICAgIDxyZWN0IGZpbGw9IndoaXRlIiB4PSIxMTAuNSIgeT0iMTIxIiB3aWR0aD0iNjU5LjI5NDQiIGhlaWdodD0iMjcyLjgzNTk0Ii8+CiAgICA8ZyBpZD0iQ2FudmFzXzFfTGF5ZXJfMSI+CiAgICAgIDx0aXRsZT5MYXllciAxPC90aXRsZT4KICAgICAgPGcgaWQ9IkdyYXBoaWNfNjMiPgogICAgICAgIDxyZWN0IHg9IjM4Ny4zOTcyIiB5PSIxNTcuMzM1OTQiIHdpZHRoPSIxMDUuNSIgaGVpZ2h0PSIzOC41IiBmaWxsPSJ3aGl0ZSIvPgogICAgICAgIDxyZWN0IHg9IjM4Ny4zOTcyIiB5PSIxNTcuMzM1OTQiIHdpZHRoPSIxMDUuNSIgaGVpZ2h0PSIzOC41IiBzdHJva2U9ImJsYWNrIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIHN0cm9rZS13aWR0aD0iMSIvPgogICAgICAgIDx0ZXh0IHRyYW5zZm9ybT0idHJhbnNsYXRlKDM5Mi4zOTcyIDE2NS45MTc5NykiIGZpbGw9ImJsYWNrIj4KICAgICAgICAgIDx0c3BhbiBmb250LWZhbWlseT0iTW9uYWNvIiBmb250LXNpemU9IjE2IiBmaWxsPSJibGFjayIgeD0iNC41NDI5NjkiIHk9IjE2Ij4wMDAwMDAwMDE8L3RzcGFuPgogICAgICAgIDwvdGV4dD4KICAgICAgPC9nPgogICAgICA8ZyBpZD0iR3JhcGhpY182MiI+CiAgICAgICAgPHJlY3QgeD0iMzg3LjM5NzIiIHk9IjE5NS44MzU5NCIgd2lkdGg9IjEwNS41IiBoZWlnaHQ9IjM4LjUiIGZpbGw9IiNjMGZmZmYiLz4KICAgICAgICA8cmVjdCB4PSIzODcuMzk3MiIgeT0iMTk1LjgzNTk0IiB3aWR0aD0iMTA1LjUiIGhlaWdodD0iMzguNSIgc3Ryb2tlPSJibGFjayIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIiBzdHJva2Utd2lkdGg9IjEiLz4KICAgICAgICA8dGV4dCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzOTIuMzk3MiAyMDQuNDE3OTcpIiBmaWxsPSJibGFjayI+CiAgICAgICAgICA8dHNwYW4gZm9udC1mYW1pbHk9Ik1vbmFjbyIgZm9udC1zaXplPSIxNiIgZmlsbD0iYmxhY2siIHg9IjQuNTQyOTY5IiB5PSIxNiI+MDAwMDAwMDAyPC90c3Bhbj4KICAgICAgICA8L3RleHQ+CiAgICAgIDwvZz4KICAgICAgPGcgaWQ9IkdyYXBoaWNfNjEiPgogICAgICAgIDxyZWN0IHg9IjM4Ny4zOTcyIiB5PSIyMzQuMzM1OTQiIHdpZHRoPSIxMDUuNSIgaGVpZ2h0PSIzOC41IiBmaWxsPSJ3aGl0ZSIvPgogICAgICAgIDxyZWN0IHg9IjM4Ny4zOTcyIiB5PSIyMzQuMzM1OTQiIHdpZHRoPSIxMDUuNSIgaGVpZ2h0PSIzOC41IiBzdHJva2U9ImJsYWNrIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIHN0cm9rZS13aWR0aD0iMSIvPgogICAgICAgIDx0ZXh0IHRyYW5zZm9ybT0idHJhbnNsYXRlKDM5Mi4zOTcyIDI0Mi45MTc5NykiIGZpbGw9ImJsYWNrIj4KICAgICAgICAgIDx0c3BhbiBmb250LWZhbWlseT0iTW9uYWNvIiBmb250LXNpemU9IjE2IiBmaWxsPSJibGFjayIgeD0iNC41NDI5NjkiIHk9IjE2Ij4wMDAwMDAwMDQ8L3RzcGFuPgogICAgICAgIDwvdGV4dD4KICAgICAgPC9nPgogICAgICA8ZyBpZD0iR3JhcGhpY182MCI+CiAgICAgICAgPHJlY3QgeD0iMzg3LjM5NzIiIHk9IjI3Mi44MzU5NCIgd2lkdGg9IjEwNS41IiBoZWlnaHQ9IjM4LjUiIGZpbGw9IndoaXRlIi8+CiAgICAgICAgPHJlY3QgeD0iMzg3LjM5NzIiIHk9IjI3Mi44MzU5NCIgd2lkdGg9IjEwNS41IiBoZWlnaHQ9IjM4LjUiIHN0cm9rZT0iYmxhY2siIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLXdpZHRoPSIxIi8+CiAgICAgICAgPHRleHQgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMzkyLjM5NzIgMjgxLjQxNzk3KSIgZmlsbD0iYmxhY2siPgogICAgICAgICAgPHRzcGFuIGZvbnQtZmFtaWx5PSJNb25hY28iIGZvbnQtc2l6ZT0iMTYiIGZpbGw9ImJsYWNrIiB4PSI0LjU0Mjk2OSIgeT0iMTYiPjAwMDAwMDAwNTwvdHNwYW4+CiAgICAgICAgPC90ZXh0PgogICAgICA8L2c+CiAgICAgIDxnIGlkPSJHcmFwaGljXzU5Ij4KICAgICAgICA8cmVjdCB4PSIzODcuMzk3MiIgeT0iMzExLjMzNTk0IiB3aWR0aD0iMTA1LjUiIGhlaWdodD0iMzguNSIgZmlsbD0iI2ZmZmZjMCIvPgogICAgICAgIDxyZWN0IHg9IjM4Ny4zOTcyIiB5PSIzMTEuMzM1OTQiIHdpZHRoPSIxMDUuNSIgaGVpZ2h0PSIzOC41IiBzdHJva2U9ImJsYWNrIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIHN0cm9rZS13aWR0aD0iMSIvPgogICAgICAgIDx0ZXh0IHRyYW5zZm9ybT0idHJhbnNsYXRlKDM5Mi4zOTcyIDMxOS45MTc5NykiIGZpbGw9ImJsYWNrIj4KICAgICAgICAgIDx0c3BhbiBmb250LWZhbWlseT0iTW9uYWNvIiBmb250LXNpemU9IjE2IiBmaWxsPSJibGFjayIgeD0iNC41NDI5NjkiIHk9IjE2Ij4wMDAwMDAwMDY8L3RzcGFuPgogICAgICAgIDwvdGV4dD4KICAgICAgPC9nPgogICAgICA8ZyBpZD0iR3JhcGhpY181OCI+CiAgICAgICAgPHJlY3QgeD0iMzg3LjM5NzIiIHk9IjM0OS44MzU5NCIgd2lkdGg9IjEwNS41IiBoZWlnaHQ9IjM4LjUiIGZpbGw9IiNjMGZmYzAiLz4KICAgICAgICA8cmVjdCB4PSIzODcuMzk3MiIgeT0iMzQ5LjgzNTk0IiB3aWR0aD0iMTA1LjUiIGhlaWdodD0iMzguNSIgc3Ryb2tlPSJibGFjayIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIiBzdHJva2Utd2lkdGg9IjEiLz4KICAgICAgICA8dGV4dCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzOTIuMzk3MiAzNTguNDE3OTcpIiBmaWxsPSJibGFjayI+CiAgICAgICAgICA8dHNwYW4gZm9udC1mYW1pbHk9Ik1vbmFjbyIgZm9udC1zaXplPSIxNiIgZmlsbD0iYmxhY2siIHg9IjQuNTQyOTY5IiB5PSIxNiI+MDAwMDAwMDA3PC90c3Bhbj4KICAgICAgICA8L3RleHQ+CiAgICAgIDwvZz4KICAgICAgPGcgaWQ9IkdyYXBoaWNfNTciPgogICAgICAgIDxyZWN0IHg9IjEzMy44MzcxOSIgeT0iMTk1LjgzNTk0IiB3aWR0aD0iMTg0LjU2IiBoZWlnaHQ9IjM4LjUiIGZpbGw9IiNjMGZmZmYiLz4KICAgICAgICA8cmVjdCB4PSIxMzMuODM3MTkiIHk9IjE5NS44MzU5NCIgd2lkdGg9IjE4NC41NiIgaGVpZ2h0PSIzOC41IiBzdHJva2U9ImJsYWNrIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIHN0cm9rZS13aWR0aD0iMSIvPgogICAgICAgIDx0ZXh0IHRyYW5zZm9ybT0idHJhbnNsYXRlKDEzOC44MzcxOSAyMDQuNDE3OTcpIiBmaWxsPSJibGFjayI+CiAgICAgICAgICA8dHNwYW4gZm9udC1mYW1pbHk9Ik1vbmFjbyIgZm9udC1zaXplPSIxNiIgZmlsbD0iYmxhY2siIHg9IjAiIHk9IjE2Ij5pcy1vZGQvaW5kZXguanM8L3RzcGFuPgogICAgICAgIDwvdGV4dD4KICAgICAgPC9nPgogICAgICA8ZyBpZD0iR3JhcGhpY181NiI+CiAgICAgICAgPHJlY3QgeD0iMTMzLjgzNzE5IiB5PSIyMzQuMzM1OTQiIHdpZHRoPSIxODQuNTYiIGhlaWdodD0iMzguNSIgZmlsbD0iI2MwZmZjMCIvPgogICAgICAgIDxyZWN0IHg9IjEzMy44MzcxOSIgeT0iMjM0LjMzNTk0IiB3aWR0aD0iMTg0LjU2IiBoZWlnaHQ9IjM4LjUiIHN0cm9rZT0iYmxhY2siIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLXdpZHRoPSIxIi8+CiAgICAgICAgPHRleHQgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTM4LjgzNzE5IDI0Mi45MTc5NykiIGZpbGw9ImJsYWNrIj4KICAgICAgICAgIDx0c3BhbiBmb250LWZhbWlseT0iTW9uYWNvIiBmb250LXNpemU9IjE2IiBmaWxsPSJibGFjayIgeD0iMCIgeT0iMTYiPmlzLW9kZC9MSUNFTlNFLm1kPC90c3Bhbj4KICAgICAgICA8L3RleHQ+CiAgICAgIDwvZz4KICAgICAgPGcgaWQ9IkdyYXBoaWNfNTUiPgogICAgICAgIDxyZWN0IHg9IjU2MS44OTcyIiB5PSIxOTUuODM1OTQiIHdpZHRoPSIxODQuNTYiIGhlaWdodD0iMzguNSIgZmlsbD0iI2ZmZmZjMCIvPgogICAgICAgIDxyZWN0IHg9IjU2MS44OTcyIiB5PSIxOTUuODM1OTQiIHdpZHRoPSIxODQuNTYiIGhlaWdodD0iMzguNSIgc3Ryb2tlPSJibGFjayIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIiBzdHJva2Utd2lkdGg9IjEiLz4KICAgICAgICA8dGV4dCB0cmFuc2Zvcm09InRyYW5zbGF0ZSg1NjYuODk3MiAyMDQuNDE3OTcpIiBmaWxsPSJibGFjayI+CiAgICAgICAgICA8dHNwYW4gZm9udC1mYW1pbHk9Ik1vbmFjbyIgZm9udC1zaXplPSIxNiIgZmlsbD0iYmxhY2siIHg9IjAiIHk9IjE2Ij5pcy1ldmVuL2luZGV4LmpzPC90c3Bhbj4KICAgICAgICA8L3RleHQ+CiAgICAgIDwvZz4KICAgICAgPGcgaWQ9IkdyYXBoaWNfNTQiPgogICAgICAgIDxyZWN0IHg9IjU2MS44OTcyIiB5PSIyMzQuMzM1OTQiIHdpZHRoPSIxODQuNTYiIGhlaWdodD0iMzguNSIgZmlsbD0iI2MwZmZjMCIvPgogICAgICAgIDxyZWN0IHg9IjU2MS44OTcyIiB5PSIyMzQuMzM1OTQiIHdpZHRoPSIxODQuNTYiIGhlaWdodD0iMzguNSIgc3Ryb2tlPSJibGFjayIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIiBzdHJva2Utd2lkdGg9IjEiLz4KICAgICAgICA8dGV4dCB0cmFuc2Zvcm09InRyYW5zbGF0ZSg1NjYuODk3MiAyNDIuOTE3OTcpIiBmaWxsPSJibGFjayI+CiAgICAgICAgICA8dHNwYW4gZm9udC1mYW1pbHk9Ik1vbmFjbyIgZm9udC1zaXplPSIxNiIgZmlsbD0iYmxhY2siIHg9IjAiIHk9IjE2Ij5pcy1ldmVuL0xJQ0VOU0UubWQ8L3RzcGFuPgogICAgICAgIDwvdGV4dD4KICAgICAgPC9nPgogICAgICA8ZyBpZD0iR3JhcGhpY181MyI+CiAgICAgICAgPHRleHQgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMzIwLjEyNzY2IDEzMSkiIGZpbGw9ImJsYWNrIj4KICAgICAgICAgIDx0c3BhbiBmb250LWZhbWlseT0iTW9uYWNvIiBmb250LXNpemU9IjE2IiBmaWxsPSJibGFjayIgeD0iMCIgeT0iMTYiPkNvbnRlbnQtYWRkcmVzc2FibGUgc3RvcmU8L3RzcGFuPgogICAgICAgIDwvdGV4dD4KICAgICAgPC9nPgogICAgICA8ZyBpZD0iR3JhcGhpY181MiI+CiAgICAgICAgPHRleHQgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTIwLjUgMTY5LjUpIiBmaWxsPSJibGFjayI+CiAgICAgICAgICA8dHNwYW4gZm9udC1mYW1pbHk9Ik1vbmFjbyIgZm9udC1zaXplPSIxNiIgZmlsbD0iYmxhY2siIHg9IjAiIHk9IjE2Ij5wcm9qZWN0XzEvbm9kZV9tb2R1bGVzPC90c3Bhbj4KICAgICAgICA8L3RleHQ+CiAgICAgIDwvZz4KICAgICAgPGcgaWQ9IkdyYXBoaWNfNDciPgogICAgICAgIDx0ZXh0IHRyYW5zZm9ybT0idHJhbnNsYXRlKDU0OC41NiAxNzIuMzg3OTQpIiBmaWxsPSJibGFjayI+CiAgICAgICAgICA8dHNwYW4gZm9udC1mYW1pbHk9Ik1vbmFjbyIgZm9udC1zaXplPSIxNiIgZmlsbD0iYmxhY2siIHg9IjAiIHk9IjE2Ij5wcm9qZWN0XzIvbm9kZV9tb2R1bGVzPC90c3Bhbj4KICAgICAgICA8L3RleHQ+CiAgICAgIDwvZz4KICAgICAgPGcgaWQ9IkxpbmVfNjQiPgogICAgICAgIDxsaW5lIHgxPSIzMTguMzk3MiIgeTE9IjIxNS4wODU5NCIgeDI9IjM3Ny40OTcyIiB5Mj0iMjE1LjA4NTk0IiBtYXJrZXItZW5kPSJ1cmwoI0ZpbGxlZEFycm93X01hcmtlcikiIHN0cm9rZT0iIzdmODA4MCIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIiBzdHJva2Utd2lkdGg9IjEiLz4KICAgICAgPC9nPgogICAgICA8ZyBpZD0iTGluZV83MSI+CiAgICAgICAgPHBhdGggZD0iTSA1NjEuODk3MiAyMTUuMDg1OTQgTCA1NTEuODk3MiAyMTUuMDg1OTQgTCA1MzEuNTE3NzUgMjE1LjI0MzQgTCA1MTguMDA5OTQgMjE1LjI0MzQgTCA1MTguMDA5OTQgMzMwLjU4NTk0IEwgNTAyLjc5NzIgMzMwLjU4NTk0IiBtYXJrZXItZW5kPSJ1cmwoI0ZpbGxlZEFycm93X01hcmtlcikiIHN0cm9rZT0iIzdmODA4MCIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIiBzdHJva2Utd2lkdGg9IjEiLz4KICAgICAgPC9nPgogICAgICA8ZyBpZD0iTGluZV83MiI+CiAgICAgICAgPHBhdGggZD0iTSAzMTguMzk3MiAyNTMuNTg1OTQgTCAzMjguMzk3MiAyNTMuNTg1OTQgTCAzNTQuNDUxMzQgMjUzLjEwNjcgTCAzNTQuNTQxMiAzNDkuODM1OTQgTCAzNTQuNTQxMiAzNjkuMDg1OTQgTCAzNzcuNDk3MiAzNjkuMDg1OTQiIG1hcmtlci1lbmQ9InVybCgjRmlsbGVkQXJyb3dfTWFya2VyKSIgc3Ryb2tlPSIjN2Y4MDgwIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIHN0cm9rZS13aWR0aD0iMSIvPgogICAgICA8L2c+CiAgICAgIDxnIGlkPSJMaW5lXzc0Ij4KICAgICAgICA8cGF0aCBkPSJNIDU2MS44OTcyIDI1My41ODU5NCBMIDU1MS44OTcyIDI1My41ODU5NCBMIDU0MC43MjMyIDI1My44ODc5NCBMIDU0MC43MjMyIDM2OS4wODU5NCBMIDUwMi43OTcyIDM2OS4wODU5NCIgbWFya2VyLWVuZD0idXJsKCNGaWxsZWRBcnJvd19NYXJrZXIpIiBzdHJva2U9IiM3ZjgwODAiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIgc3Ryb2tlLXdpZHRoPSIxIi8+CiAgICAgIDwvZz4KICAgIDwvZz4KICA8L2c+Cjwvc3ZnPgo=" alt="Ubuntu terminal displaying node installed" width="800px" />
</p>

When using npm, if you have 100 projects using a dependency, you will have 100 copies of that dependency saved on disk. With pnpm, the dependency will be stored in a content-addressable store, so:

1. If you depend on different versions of the dependency, only the files that differ are added to the store. For instance, if it has 100 files, and a new version has a change in only one of those files, pnpm update will only add 1 new file to the store, instead of cloning the entire dependency just for the singular change.

2. All the files are saved in a single place on the disk. When packages are installed, their files are hard-linked from that single place, consuming no additional disk space. This allows you to share dependencies of the same version across projects.

As a result, you save a lot of space on your disk proportional to the number of projects and dependencies, and you have a lot faster installations!

## Installation

Please refer to [their docs](https://pnpm.io/installation) for installation instructions.