class Solution {
    public List<String> readBinaryWatch(int turnedOn) {
        List<String> result = new ArrayList<>();

        for (int hour = 0; hour < 12; hour++) {

            for (int minute = 0; minute < 60; minute++) {

                // Count total number of set bits (1s) in hour and minute
                // Integer.bitCount(x) returns number of 1s in binary form of x
                int totalBits = Integer.bitCount(hour) + Integer.bitCount(minute);

                // If total LEDs turned on equals the given turnedOn value
                if (totalBits == turnedOn) {

                    String time = hour + ":" +
                            (minute < 10 ? "0" + minute : minute);

                    result.add(time);
                }
            }
        }

        return result;
    }
}
