def findTwoWords(L, N):
    res = []
    word = ""
    for i in range(L.count("")):
        L.remove("")
    for item in L:
        if len(item) == N:
            for sub in L:
                if sub in item and item.index(sub) == 0:
                    word = item.replace(sub, "", 1)
                    if word in L and word != sub:
                        res.append(item)
                        break
                    elif word in L and sub == word:
                        if L.count(sub) == 1:
                            continue
                        elif L.count(sub) > 1:
                            res.append(item)
                            break
                    else:
                        continue
                else:
                    continue
        else:
            continue
    return res
