#include <stdio.h>

int a[20], n, target, s[20], top = 0, found = 0;

void solve(int i, int sum)
{
    if (i == n) {
        if (sum == target) {
            for (int j = 0; j < top; j++)
                printf("%d ", s[j]);
            printf("\n");
            found = 1;
        }
        return;
    }

    solve(i + 1, sum);

    s[top++] = a[i];
    solve(i + 1, sum + a[i]);
    top--;
}

int main()
{
    scanf("%d", &n);

    for (int i = 0; i < n; i++)
        scanf("%d", &a[i]);

    scanf("%d", &target);

    solve(0, 0);

    if (!found)
        printf("-1\n");
}
