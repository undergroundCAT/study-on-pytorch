# study-on-pytorch
关于torchvision.transforms.ToTensor的问题


在官方文档中，class torchvision.transforms.ToTensor是把一个取值范围在0-255的np.array转化成0-1之间的torch.FloadTensor。

这里可以将数组自动归一化，官方的例子是：

data = np.random.randint(0, 255, size=300)
img = data.reshape(10,10,3)
print(img.shape)
img_tensor = transforms.ToTensor()(img) # 转换成tensor
print(img_tensor)
