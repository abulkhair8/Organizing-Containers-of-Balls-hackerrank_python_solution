def organizingContainers(container):
    all_colums = []
    for i in range(n):
        colums = sum(container[i])
        all_colums.append(colums)
    for i in range(n):
        row = 0
        for j in range(n):
            row += container[j][i]
        if row in all_colums:
            continue
        else:
            return "Impossible"
    return "Possible"
