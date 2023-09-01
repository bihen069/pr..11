# pr..11
    public void testArrayCopy99(){
        int size = 100000;
        int[] array = new int[size];
        int[] arraydest = new int[size];

        for(int i=0;i<array.length;i++){
            array[i] = i;
        }
        long start = System.currentTimeMillis();
        for (int k=0;k<1000;k++){
            for(int i=0;i<size;i++){
                arraydest[i] = array[i];
            }
        }
        long useTime = System.currentTimeMillis()-start;
        System.out.println("useTime:"+useTime);
    }
