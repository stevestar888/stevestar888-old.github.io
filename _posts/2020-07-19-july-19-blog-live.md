---
layout: post
title: July 19—the day this blog goes live
subtitle: Today is an exceptional Sunday, because this website & blog is now live
cover-img: /assets/img/spiderman.jpg
thumbnail-img: /assets/img/new-thumb.png
share-img: /assets/img/path.jpg
tags: [admin, happy, music]
---

# Weclome! 
I will put leet here. And thoughts and ideas.

## Ideas
Ideas will go here.
Ideas will go here.
Ideas will go here.
Ideas will go here.
Ideas will go here.
Ideas will go here.

## Code 
```vector<int> pancakeSort( const vector<int>& arr ) 
{
  vector<int> result(arr);
  
  int n = result.size();
  
  int cm = getMax(result, n);
  
  int cnt = 1;
  
  for (int i = 0; cnt <= result.size(); i++) {
     if (result[i] == cm) {
       flip(result, i);
       flip(result, n-cnt);
       cm = getMax(result, n-cnt);
       i = 0;
       cnt++;
     }
      
  }
  
  return result;
  
}

int main() {
  
  vector<int> a = {1, 5, 4, 3, 2};
  
  vector<int> res = pancakeSort(a);
  
  for (auto i : res) cout << i  << " ";
  
  return 0;
}
```