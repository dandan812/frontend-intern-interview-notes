
实现一个函数findKthLargest，在未排序的数组中找 到第k个最大的元素。
const findKthLargest = (nums, k) => nums.sort((a, b) => b - a)[k - 1]



递归查找指定 id
const data = [
  {
    id: 1,
    name: 'A',
    children: [
      {
        id: 2,
        name: 'B',
        children: [
          { id: 3, name: 'C' }
        ]
      }
    ]
  },
  {
    id: 4,
    name: 'D'
  }
]


function findById(list, targetId) {
  for (const item of list) {
    if (item.id === targetId) {
      return item
    }
    if (item.children?.length) {
      const result = findById(item.children, targetId)
      if (result) return result
    }
  }
  return null
}

const res = findById(data, 3)
console.log(res)
// { id: 3, name: 'C' }



