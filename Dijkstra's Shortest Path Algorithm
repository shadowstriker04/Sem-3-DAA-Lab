#include <limits.h> 
#include <stdio.h>
#define MAX 20
int V, E;
int graph[MAX][MAX];
#define INFINITY 99999

void dijkstra(int G[MAX][MAX], int n, int startnode) {
	int dist[MAX], visited[MAX], parent[MAX];
	int i, j, u, min;

	for(i = 1; i <= n; i++) {
		dist[i] = INFINITY;
		visited[i] = 0;
		parent[i] = -1;
	}

	dist[startnode] = 0;

	for(i = 1; i <= n; i++) {
		min = INFINITY;
		u = -1;

		for(j = 1; j <= n; j++) {
			if(!visited[j] && dist[j] < min) {
				min = dist[j];
				u = j;
			}
		}

		if(u == -1)
			break;

		visited[u] = 1;

		for(j = 1; j <= n; j++) {
} 
