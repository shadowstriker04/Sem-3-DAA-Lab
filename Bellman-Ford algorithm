#include <stdio.h>
#include <limits.h>

#define INF INT_MAX

struct Edge {
    int u, v, w;
};

void printPath(int parent[], int v) {
    if (parent[v] == -1) {
        printf("%d", v);
        return;
    }

    printPath(parent, parent[v]);
    printf("->%d", v);
}

int main() {
    int V, E;

    scanf("%d", &V);
    scanf("%d", &E);

    struct Edge edges[E];

    for (int i = 0; i < E; i++) {
        scanf("%d %d %d",
              &edges[i].u,
              &edges[i].v,
              &edges[i].w);
    }

    int src;
    scanf("%d", &src);
}
