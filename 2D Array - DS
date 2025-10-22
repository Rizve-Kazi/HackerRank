#include <bits/stdc++.h>
using namespace std;

int main() {
    int n = 6, m = 6;
    vector<vector<int>> v(n, vector<int>(m));

    for (int i = 0; i < n; i++) {
        for (int j = 0; j < m; j++) {
            cin >> v[i][j];
        }
    }

    vector<int> arr;

    for (int i = 0; i < n - 2; i++) {
        for (int j = 0; j < m - 2; j++) {
            int sum = v[i][j] + v[i][j + 1] + v[i][j + 2]
                    + v[i + 1][j + 1]
                    + v[i + 2][j] + v[i + 2][j + 1] + v[i + 2][j + 2];
            arr.push_back(sum);
        }
    }

    int ans = *max_element(arr.begin(), arr.end());
    cout << ans << endl;
}
