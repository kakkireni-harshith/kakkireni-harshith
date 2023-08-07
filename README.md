def binary_search(arr,pivot):
  low=0
  high=len(arr)-1
  while low<=high:
    mid=(low+high)//2
    if arr[mid]==pivot:
      return("element is found at {}position".format(mid+1))
      break
    elif pivot<arr[mid]:
      high=mid-1
    else:
      low=mid+1
arr=[1,2,3,4,5,6,7,9,8]
pivot=7
print(binary_search(arr,pivot))
