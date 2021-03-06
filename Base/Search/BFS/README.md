# BFS

## BFS using Queue

```c++
void bfs(int start) {
    bool visited[SIZE];
    fill_n(visited, SIZE, false);

    queue<int> q;
    q.push(start);
    visited[start] = true;

    while (!q.empty()) {
        int cur = q.front();
        q.pop();

        for (int i = 0; i < 4; i++) {
            // Do something
            int next; // Set next
            if (!visited[next]) {
                visited[next] = true;
                q.push(next);
            }
        }
    }
}
```

### BFS를 이용하여 풀 수 있는 문제

- [BOJ - 구슬 탈출 2](../../BOJ/Samsung/13460_구슬탈출2/)
- [BOJ - 연구소](../../BOJ/Samsung/14502_연구소/)