# Iris_SuanPhueng
featureA = np.load('LG_L_enroll.npy',allow_pickle=True)

featureB = np.load('LG_L_test.npy',allow_pickle=True)


# Simplest Hamming Distance

C = np.logical_xor(featureA[0], featureB[1])

HD = np.sum(C == 1)/featureA[0].size

print(HD)
